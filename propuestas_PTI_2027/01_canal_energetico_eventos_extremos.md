# Proyecto 1. El canal energético de los eventos meteorológicos extremos en México

Propuesta de entregable 2027 para el proyecto 10 del Programa de Trabajo DGIE 2026-2027 ("Investigación sobre economía ambiental y finanzas sustentables").
Versión 1, 29 de septiembre de 2026. Uso interno.

## 0. Ficha para el PTI

| Campo | Contenido |
|---|---|
| Dirección | [Dirección del proponente] |
| Título | El canal energético de los eventos meteorológicos extremos en México |
| Entregable | Nota técnica |
| Trimestre | 2027 T3 (con margen a T4) |
| Línea del proyecto 10 con la que dialoga | Eventos meteorológicos extremos (DME, entregables ii y iii de 2026) |

**Párrafo para el PTI (137 palabras):**

> [Dirección] El canal energético de los eventos meteorológicos extremos en México. Se estudia cómo los eventos meteorológicos extremos se transmiten al sistema energético mexicano y, a través de él, a los precios de los combustibles, a la balanza comercial energética y a las finanzas públicas. Para ello, se construye una base de eventos de calor y frío extremos, sequía y huracanes a partir del reanálisis ERA5 de Copernicus y de los registros de trayectorias de ciclones de la NOAA, y se vincula con datos horarios de demanda, generación y precios del mercado eléctrico (CENACE), con las estadísticas de producción, importación y ventas de gas natural y petrolíferos (SENER y Pemex) y con los precios y estímulos fiscales de las gasolinas y el diésel (CNE y SHCP). Se estiman modelos de panel y de proyecciones locales que explotan la variación regional y temporal de los eventos. Se incluye el canal externo: los huracanes que cierran refinerías en la costa estadounidense del Golfo y encarecen la factura de importación de México. Se elaborará una nota técnica. (2027 T3)

## 1. Pregunta y motivación

**Pregunta.** ¿Cuánto cuesta un evento meteorológico extremo al sistema energético mexicano y cómo llega ese costo a los precios, a la balanza comercial y a las finanzas públicas?

**Por qué importa para el Banco.** El sector energético es el canal más directo por el que el clima se vuelve inflación y cuenta corriente. Una ola de calor sube la demanda eléctrica, obliga a quemar combustóleo y gas caro, y eleva los precios marginales del mercado eléctrico. Una sequía prolongada retira generación hidroeléctrica y la sustituye con térmica importada. Un frente frío en Texas corta el gas que alimenta la generación del norte del país, como ocurrió en febrero de 2021. Un huracán en la costa estadounidense del Golfo cierra refinerías, abre los diferenciales de gasolina y diésel y encarece la factura de importación de petrolíferos de México, y con ella el costo del estímulo al IEPS. Cada uno de estos episodios toca precios administrados y de mercado que están en el INPC, toca la balanza petrolera y toca el presupuesto.

**El hueco.** Los entregables ii y iii de DME miden la frecuencia de los eventos y su efecto sobre el sector real. Ninguno de los entregables del proyecto 10 sigue la cadena energía, precios y finanzas públicas. La literatura internacional sobre temperatura y demanda eléctrica es amplia para Estados Unidos y para algunos países en desarrollo, pero para México es escasa, y no hay trabajo que junte el canal doméstico (electricidad y gas) con el canal externo (refinación en el Golfo) en un solo marco.

**Qué aporta.** Tres cosas. Una base de eventos extremos orientada a energía, con definiciones que corresponden a los umbrales que importan al sistema eléctrico (temperatura máxima, días consecutivos, región de control). Un conjunto de elasticidades y respuestas dinámicas estimadas con datos mexicanos: demanda y precios eléctricos ante calor extremo, generación hidroeléctrica ante sequía, importaciones y precios de gas ante frío extremo, importaciones y precios de petrolíferos ante huracanes en el Golfo. Y una traducción de esas respuestas a magnitudes que el Banco sigue: componente energético del INPC, balanza comercial energética y costo fiscal del estímulo a los combustibles.

## 2. Relación con el objetivo del proyecto 10 y con las líneas existentes

El objetivo del proyecto 10 habla de la interacción de los eventos climáticos inesperados con la actividad económica y los mercados, en particular de México. Esta propuesta cubre el canal que falta: el energético. Se apoya en la misma fuente meteorológica que usa DME (ERA5), lo que facilita comparar definiciones de evento y resultados, pero no depende de su base. La sección 4 explica cómo se construye una propia y cuánto cuesta.

Complementa a los tres entregables existentes sin duplicarlos:

- Con la base de eventos de DME (2026 T3), comparte la fuente y puede validar definiciones. Si DME comparte su base, se usa como robustez; si no, el proyecto no se detiene.
- Con la nota de DME sobre el sector real (2026 T3), se distingue por el objeto: aquí las variables dependientes son energéticas y de precios, no de producción.
- Con el proyecto agrícola de DASPERI (2027 T4), comparte el interés en la sequía, pero mira su efecto en la generación hidroeléctrica y en el consumo de combustibles, no en la producción agrícola.

## 3. Antecedentes y literatura

[PENDIENTE: se completa con la verificación de referencias.]

## 4. Datos

[PENDIENTE: inventario de fuentes con condiciones de acceso verificadas.]

## 5. Metodología

### 5.1 Definición de eventos

Los eventos se definen sobre datos diarios de ERA5 agregados a las regiones de control del sistema eléctrico (nueve gerencias de control regional del CENACE: Central, Oriental, Occidental, Noroeste, Norte, Noreste, Peninsular, Baja California y Baja California Sur) con ponderadores de población del marco geoestadístico del INEGI. Se usa una climatología de referencia de 1991 a 2020 para los umbrales.

| Evento | Variable de ERA5 | Definición operativa | Robustez |
|---|---|---|---|
| Calor extremo | Temperatura máxima diaria a 2 m | Tres o más días consecutivos por arriba del percentil 95 de la climatología local del mes | Percentil 90 y 97.5; umbral absoluto de 35 °C; grados día de enfriamiento |
| Frío extremo | Temperatura mínima diaria a 2 m | Dos o más días por abajo del percentil 5 | Percentil 2.5; incluir la temperatura en Texas para el canal del gas |
| Sequía | Precipitación y evapotranspiración potencial | Índice estandarizado de precipitación y evapotranspiración (SPEI) a 3, 6 y 12 meses por región y por cuenca de las presas hidroeléctricas | Monitor de Sequía de México de CONAGUA; almacenamiento de presas |
| Lluvia extrema | Precipitación diaria | Percentil 99 de la climatología local | Percentil 95 |
| Huracán | Trayectorias HURDAT2 e IBTrACS | Municipios dentro del radio de vientos de tormenta tropical o de huracán; para el canal externo, tocar tierra en Texas o Luisiana con categoría 1 o mayor | Categoría 3 o mayor; incluir tormentas tropicales |

Los eventos se agregan a la frecuencia de cada variable dependiente: horaria y diaria para el mercado eléctrico, semanal para precios de combustibles y estímulos, mensual para importaciones y generación por tecnología.

### 5.2 Canal doméstico: electricidad

**Demanda.** Con la demanda horaria por región de control se estima una función de respuesta no lineal a la temperatura, con intervalos (bins) de temperatura y efectos fijos de región, hora, día de la semana, mes y año. El interés está en los intervalos altos y en la interacción con la duración del evento (primer día contra tercer día de la ola de calor). Se estima también cómo ha cambiado la pendiente en el tiempo, como medida de adopción de aire acondicionado.

**Oferta y mezcla de generación.** Con la generación horaria por tecnología se estima cómo cambia la mezcla durante los eventos: cuánto sube la térmica convencional y el combustóleo, cuánto baja la hidroeléctrica en sequía, y qué pasa con la disponibilidad térmica en calor extremo (las plantas de ciclo combinado pierden eficiencia con temperatura alta).

**Precios.** Con los precios marginales locales horarios por nodo o por zona de carga se estima el efecto del evento sobre el precio promedio y sobre el precio en horas pico. Este es el vínculo con el costo de suministro de la CFE y, en última instancia, con las tarifas.

**Gas natural.** Con las importaciones mensuales por ducto y los precios de referencia (índice nacional de gas natural y precios de los centros del sur de Texas), se estima el efecto de los frentes fríos en el norte de México y en Texas sobre volúmenes y precios. El episodio de febrero de 2021 se trata como estudio de caso separado, porque es único en magnitud.

### 5.3 Canal externo: huracanes y refinación en el Golfo

Se identifican los huracanes que tocaron tierra en Texas o Luisiana desde 1990 con categoría 1 o mayor y se documenta, con los reportes de la Administración de Información Energética de Estados Unidos, la capacidad de refinación que cerró y por cuánto tiempo. Con datos semanales se estiman proyecciones locales del efecto de cada evento sobre:

1. la utilización de refinerías en el distrito 3 (costa del Golfo);
2. los diferenciales de gasolina y diésel frente al crudo en la costa del Golfo;
3. las importaciones mexicanas de gasolina y diésel (volumen y valor unitario);
4. los precios en estación en México;
5. el estímulo semanal al IEPS y su costo, calculado con los volúmenes de venta.

La secuencia de tiempos importa: el diferencial reacciona en días, la importación en semanas, el estímulo en la semana siguiente. Por eso las proyecciones locales van de una a doce semanas.

### 5.4 Traducción a magnitudes macro

Con las respuestas estimadas se construyen tres cuentas por tipo de evento y por región:

- **Precios.** Contribución al componente de energéticos del INPC vía electricidad (tarifas de alto consumo y comercial), gas LP y gasolinas.
- **Balanza.** Cambio en la factura de importación de gas y petrolíferos.
- **Finanzas públicas.** Costo adicional del estímulo al IEPS y costo de generación de la CFE.

Se cierra con un ejercicio de exposición: qué habría pasado si el verano de 2023 (calor extremo y sequía) hubiera coincidido con un huracán mayor en el Golfo, usando las respuestas estimadas.

### 5.5 Identificación

El clima es exógeno a las variables energéticas de corto plazo, así que la identificación descansa en efectos fijos que absorben estacionalidad y tendencias por región, y en la variación entre regiones dentro del mismo periodo. Los riesgos son dos: la adaptación (la respuesta cambia con el tiempo) y la simultaneidad de eventos (calor y sequía suelen coincidir). El primero se trata con interacciones con el tiempo; el segundo, estimando los eventos de forma conjunta y reportando efectos condicionales.

## 6. Resultados esperados

1. Una base de eventos meteorológicos extremos por región de control eléctrico, con definiciones documentadas y reproducibles.
2. Elasticidades de la demanda eléctrica a la temperatura por región y su cambio en el tiempo.
3. Efecto de las olas de calor sobre precios marginales y sobre el uso de combustóleo y gas.
4. Efecto de la sequía sobre la generación hidroeléctrica y su sustitución por térmica.
5. Efecto de los frentes fríos sobre importaciones y precios de gas.
6. Respuesta dinámica de diferenciales, importaciones, precios en estación y estímulo al IEPS ante huracanes en el Golfo.
7. Una cuenta de exposición: cuánto cuesta cada tipo de evento en inflación, balanza y presupuesto, y un escenario de coincidencia.

## 7. Entregables y calendario

| Periodo | Actividad | Producto intermedio |
|---|---|---|
| 2026 T4 | Descarga de ERA5, CENACE, SIE, BDI, CNE, SHCP, EIA y HURDAT2. Construcción de la base de eventos. | Base de eventos y documentación |
| 2027 T1 | Estimaciones del canal doméstico (demanda, generación, precios, gas) | Cuadros de resultados |
| 2027 T2 | Estimaciones del canal externo y traducción macro | Versión preliminar de la nota |
| 2027 T3 | Redacción, seminario interno, ajustes | Nota técnica |
| 2027 T4 | Margen para comentarios y versión final | Nota técnica final |

## 8. Riesgos y mitigación

| Riesgo | Probabilidad | Mitigación |
|---|---|---|
| El acceso a datos horarios del CENACE cambia o se restringe | Baja | Descargar y respaldar todo al inicio; las series del SIE mensual son el respaldo |
| Cola de descarga de ERA5 lenta | Media | Restringir el periodo a 1991-2025, usar el producto diario derivado, o la API de Open-Meteo como respaldo |
| Pocos huracanes mayores para el canal externo | Media | Usar datos semanales y todos los eventos de 1990 a 2025; complementar con tormentas tropicales |
| Simultaneidad de calor y sequía | Alta | Estimación conjunta y efectos condicionales |
| Cambios institucionales (CRE a CNE, CNH a CNE) rompen las series | Media | Documentar los empalmes; guardar las versiones históricas de los archivos |

## 9. Sinergias

- DME: misma fuente meteorológica; comparar definiciones de evento. Intercambio deseable, no necesario.
- DASPERI: la sequía en la generación hidroeléctrica y la sequía en la agricultura comparten cuencas.
- Reporte semanal de mercados petroleros: la infraestructura de datos de SENER, CNE, SHCP y EIA ya está armada en el pipeline semanal; este proyecto la reutiliza y le devuelve un módulo de eventos extremos.

## 10. Referencias

[PENDIENTE: se completa con la verificación de referencias.]
