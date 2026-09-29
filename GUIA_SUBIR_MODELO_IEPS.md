# Guía para subir el material del modelo de IEPS a combustibles

Esta sesión de Claude corre en la nube y solo ve lo que está en el repositorio `fjdrl89/projects_bdm`.
No puede abrir rutas de Windows ni OneDrive. Para auditar el modelo hay que traer aquí el contenido de:

```
C:\Users\fjdrl\OneDrive\Documentos\BdM_FJ\1_Energy&Climate\1_1_Sector_Energetico\2_IEPS_Gasolinas
```

y en particular la subcarpeta `Modelo_IEPS`.

Hay dos caminos. Elige uno.

| Camino | Cuándo conviene | Qué requiere |
|---|---|---|
| **A. Claude Code local** en tu máquina Windows | El material es sensible o pesa mucho; no quieres subir nada a GitHub | Instalar la app de escritorio de Claude Code o el CLI |
| **B. Subir la carpeta al repositorio** | Quieres que esta sesión en la nube lo audite y quede versionado | Un navegador (o Git en Windows) |

---

## 0. Antes de subir nada: el repositorio es PÚBLICO

`fjdrl89/projects_bdm` es público hoy. Todo lo que subas lo puede ver cualquiera con la liga.
Si el modelo o sus datos son material interno de trabajo, **cambia el repositorio a privado antes de subir**:

1. En GitHub abre el repositorio, pestaña **Settings**.
2. Baja hasta **Danger Zone**, botón **Change repository visibility**, elige **Private** y confirma.

La sesión en la nube sigue teniendo acceso al repositorio aunque sea privado, porque el acceso viene de la
app de Claude instalada en tu cuenta, no de que sea público.

---

## 1. Inventario rápido (opcional, pero ayuda)

Antes de subir, corre esto en PowerShell y pega el resultado en el chat. Así sé de antemano qué hay
(tipos de archivo, tamaños, fechas) y detectamos archivos demasiado grandes:

```powershell
$raiz = "C:\Users\fjdrl\OneDrive\Documentos\BdM_FJ\1_Energy&Climate\1_1_Sector_Energetico\2_IEPS_Gasolinas"
Get-ChildItem -Path $raiz -Recurse -File |
  Select-Object @{n='Ruta';e={$_.FullName.Replace($raiz,'')}},
                @{n='MB';e={[math]::Round($_.Length/1MB,2)}},
                LastWriteTime |
  Sort-Object MB -Descending |
  Format-Table -AutoSize | Out-String -Width 300 | Set-Content "$env:USERPROFILE\Desktop\inventario_ieps.txt"
```

Abre `inventario_ieps.txt` del escritorio y pégalo aquí.

**Archivos de OneDrive "solo en línea".** Si en el explorador el archivo tiene el ícono de nube, no está
descargado. Clic derecho sobre la carpeta `2_IEPS_Gasolinas` y **Conservar siempre en este dispositivo**
antes de subir; si no, se suben archivos vacíos o falla la carga.

---

## 2. Límites de tamaño que importan

| Límite | Valor | Consecuencia |
|---|---|---|
| Archivo por el navegador | 25 MB | Más grande no se puede arrastrar; usa Git (sección 4) |
| Archivo por Git | 100 MB | Más grande GitHub lo rechaza |
| Archivos por carga en navegador | 100 | Si hay más, se sube en varias tandas o por Git |

Si hay archivos entre 25 y 100 MB (bases de datos crudas, por ejemplo), usa el camino por Git.
Si hay archivos de más de 100 MB, no los subas: comprímelos en `.zip` si con eso bajan del límite, o déjalos
fuera y dime qué son y de dónde salen; con la descripción y una muestra basta para la auditoría.
**No uses Git LFS**: esta sesión no puede descargar objetos LFS.

---

## 3. Camino B.1: subir desde el navegador (sin instalar nada)

1. Abre en GitHub `https://github.com/fjdrl89/projects_bdm`.
2. Arriba a la izquierda, en el selector de ramas, elige la rama **`claude/sweet-cannon-a7bt4g`**
   (es la rama de esta sesión; ahí ya existe la carpeta `ieps_gasolinas/`).
3. Entra a la carpeta **`ieps_gasolinas`**.
4. Botón **Add file** y luego **Upload files**.
5. En el explorador de Windows abre `2_IEPS_Gasolinas`, selecciona todo su contenido con Ctrl+A
   (el contenido, no la carpeta) y arrástralo a la zona *Drag files here*. Chrome y Edge conservan
   la estructura de subcarpetas, incluida `Modelo_IEPS`.
6. Espera a que suban todos. Si hay más de 100 archivos, sube `Modelo_IEPS` primero y el resto en una
   segunda tanda.
7. Abajo, en *Commit changes*, deja marcado **Commit directly to the `claude/sweet-cannon-a7bt4g` branch**
   y da **Commit changes**.
8. Regresa a este chat y escribe "ya subí". Yo hago `git pull` y empiezo la auditoría.

---

## 4. Camino B.2: subir con Git desde PowerShell (para archivos grandes o muchos archivos)

Requiere Git para Windows (`git --version` en PowerShell lo confirma; si no está, se instala de
`git-scm.com`).

```powershell
# 1. Clonar el repositorio (una sola vez) en una carpeta fuera de OneDrive
cd C:\Users\fjdrl\Documents
git clone https://github.com/fjdrl89/projects_bdm.git
cd projects_bdm

# 2. Pararse en la rama de esta sesión
git fetch origin
git checkout claude/sweet-cannon-a7bt4g

# 3. Copiar el material (robocopy conserva la estructura y salta archivos temporales)
$origen = "C:\Users\fjdrl\OneDrive\Documentos\BdM_FJ\1_Energy&Climate\1_1_Sector_Energetico\2_IEPS_Gasolinas"
robocopy $origen ".\ieps_gasolinas" /E /XF "~$*" "Thumbs.db" "desktop.ini" /XD ".git" "__pycache__" ".ipynb_checkpoints"

# 4. Revisar que no haya archivos de más de 95 MB
Get-ChildItem ".\ieps_gasolinas" -Recurse -File | Where-Object Length -gt 95MB | Select-Object FullName, @{n='MB';e={[math]::Round($_.Length/1MB,1)}}

# 5. Subir
git add ieps_gasolinas
git commit -m "Material del modelo de IEPS a combustibles"
git push -u origin claude/sweet-cannon-a7bt4g
```

Si el paso 4 muestra algo, mueve esos archivos fuera de `ieps_gasolinas` antes del `git add`.
Al terminar, avísame en el chat.

---

## 5. Camino A: Claude Code local (sin subir nada)

Si prefieres que nada salga de tu máquina:

1. Instala la app de escritorio de Claude Code (o el CLI) en Windows.
2. Ábrela con la carpeta `2_IEPS_Gasolinas` como directorio de trabajo.
3. Pide ahí mismo la auditoría. Claude lee los archivos directamente de OneDrive y no hay que subir nada.

La desventaja es que el resultado de esta sesión no se aprovecha, pero puedes pegarle el mismo mensaje.

---

## 6. Qué necesito que venga en la carga para auditar bien

En orden de importancia:

1. **El modelo en sí**: el libro de Excel, el código (Python, R, Stata, EViews, Matlab) o lo que sea que produce el pronóstico.
2. **Los insumos**: las series que alimenta (precios de referencia, tipo de cambio, cuotas, estímulos del DOF, volúmenes, recaudación de Hacienda), o al menos una muestra y la lista de fuentes.
3. **Salidas**: pronósticos que ya has publicado o guardado, para contrastarlos con lo observado.
4. **Documentación y notas**: metodología, notas técnicas, bitácoras, versiones anteriores del modelo, correos o minutas donde se discutió el diseño.
5. **Lo que ya evaluamos antes**: si hay reportes de errores, pruebas fuera de muestra, comparaciones con Hacienda o con el CGPE, inclúyelos.

Formatos que puedo leer directamente: `.xlsx`, `.xlsm`, `.csv`, `.py`, `.ipynb`, `.R`, `.do`, `.dta`, `.m`, `.docx`, `.pdf`, `.md`, `.txt`.
Formatos que no puedo abrir: archivos de EViews (`.wf1`). Si el modelo está en EViews, exporta el workfile a Excel
(`File > Save As > Excel`) y guarda los programas (`.prg`) como texto; ambos súbelos junto al `.wf1`.

---

## 7. Después de subir

Escribe en el chat "ya subí" (y pega el inventario si lo generaste). A partir de ahí la auditoría corre
sobre el repositorio: se revisa estructura, fórmulas, datos, supuestos, pruebas fuera de muestra y se
entrega la evaluación en un documento dentro de `ieps_gasolinas/`.
