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

**Párrafo para el PTI (176 palabras):**

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

**Temperatura y demanda eléctrica.** La relación entre temperatura y consumo eléctrico es una de las respuestas mejor documentadas de la economía del clima. Deschênes y Greenstone (2011) estiman con datos anuales de Estados Unidos que el consumo residencial de energía sube con los días de calor extremo. Auffhammer, Baylis y Hausman (2017) muestran con datos horarios que el cambio climático afecta más a la demanda pico que a la demanda promedio, lo que importa para el costo de generación. Wenz, Levermann y Auffhammer (2017) estiman la curva horaria de respuesta de la carga a la temperatura para 35 países europeos, y su método es la plantilla para hacerlo con las regiones de control del CENACE. Auffhammer y Mansur (2014) revisan la literatura empírica. Rode y coautores (2021) llevan el ejercicio a escala mundial. Para México, Davis y Gertler (2015) usan microdatos de hogares mexicanos para estimar cómo la adopción de aire acondicionado amplifica la respuesta del consumo a la temperatura; es la referencia mexicana principal. Hay trabajos recientes con paneles estatales y municipales para México (Sustainability, 2021; Atmósfera, 2022; Environment, Development and Sustainability, 2024), que confirman que el consumo sube con la temperatura y más en los estados cálidos, pero ninguno usa datos horarios del mercado eléctrico ni sigue el efecto hasta precios y combustibles.

**Huracanes y refinación en el Golfo.** Los informes del Servicio de Investigación del Congreso de Estados Unidos sobre Katrina y Rita (2005) documentan que hasta una tercera parte de la capacidad de refinación del país quedó fuera de operación. La Administración de Información Energética documentó que Harvey (2017) redujo las entradas a refinerías del distrito 3 en cerca de una tercera parte en una semana y que Ida (2021) cerró nueve refinerías de Luisiana con cerca del 13 por ciento de la capacidad nacional. Un artículo de 2025 en Environmental Research Letters estudia los cierres anticipados que se disparan con el pronóstico, antes de que el huracán toque tierra, que es el canal que más importa para los diferenciales. Lewis (2009) muestra que los picos de precios al mayoreo después de Rita tuvieron efectos duraderos en el precio al menudeo; la referencia queda por confirmar.

**Episodios mexicanos.** La tormenta invernal de febrero de 2021 en Texas cortó el suministro de gas al norte de México y dejó sin electricidad a millones de usuarios; el informe del Laboratorio Nacional de Argonne (2021) documenta el lado texano, y las notas de prensa de la época el lado mexicano, incluida la orden del gobernador de Texas de priorizar el gas para generadores del estado. La sequía de 2023 redujo la generación hidroeléctrica de la CFE a cerca de la mitad de la de 2022 según cifras de prensa que citan a la empresa, y que hay que confirmar con los datos del CENACE.

**Trabajo del Banco.** El Documento de Investigación 2023-16 (Arellano-González, Juárez-Torres y Zazueta-Borboa) estima el efecto de choques de temperatura y precipitación sobre precios y productividad de granos básicos, con el mismo tipo de identificación que propone este proyecto. El informe del Banco con el PNUMA y el PNUD (2020) sobre riesgos climáticos del sistema financiero es el marco institucional. El Reporte sobre las Economías Regionales ha incluido recuadros con la opinión empresarial sobre el impacto de eventos climáticos. Los entregables ii y iii de DME en el PTI 2026 son el antecedente más cercano.

## 4. Datos

### 4.1 Criterio y advertencia

Todo lo que necesita el proyecto está en fuentes públicas o en la terminal financiera del Banco. No hay que pedir nada a otra dirección. La única excepción es la base de eventos de DME, que serviría como robustez, no como insumo.

Las direcciones y condiciones de acceso se confirmaron el 29 de septiembre de 2026 con resultados de buscadores. Desde el entorno donde se preparó esta propuesta no se pudieron abrir las páginas oficiales, así que antes de arrancar conviene abrir cada fuente desde un equipo del Banco. Lo que no se pudo confirmar está marcado con "por confirmar".

### 4.2 Inventario de fuentes

**A. Clima**

| Fuente | Contenido | Periodo y frecuencia | Acceso y costo | Formato y volumen | Complejidad | Estado |
|---|---|---|---|---|---|---|
| ERA5 horario, niveles de superficie (Copernicus CDS) | Temperatura a 2 m, precipitación, viento, presión; malla de 0.25° | 1940 a la fecha, horario, rezago de cinco días | Cuenta gratuita de ECMWF, aceptar licencia por conjunto, token y cliente `cdsapi`; licencia CC BY 4.0 | GRIB o NetCDF; para la caja de México, 15 a 30 GB por variable para 1940-2025; 1991-2025 pesa una tercera parte | Media: tope de 120 mil campos por solicitud, cola de espera, conversión de UTC a hora local | Confirmado por búsqueda |
| ERA5 estadísticas diarias derivadas (CDS) | Máximo, mínimo, media y suma diaria de las mismas variables, con opción de huso horario | 1940 a la fecha, diario | Igual que ERA5 | NetCDF; 1 a 2 GB por variable para todo el periodo | Baja a media: se calcula al vuelo, se pide por año | Confirmado por búsqueda |
| ERA5 series de tiempo por punto (CDS, desde marzo de 2025) | Serie horaria completa para una coordenada en una sola solicitud | 1940 a la fecha | Igual que ERA5 | CSV o NetCDF, ligero | Baja: ideal para una ciudad por región de control | Confirmado por búsqueda |
| ERA5-Land (CDS) | Igual que ERA5 sobre tierra, malla de 0.1° | 1950 a la fecha | Igual que ERA5 | Seis veces más pesado que ERA5 | Media a alta | Solo si hace falta detalle; no se recomienda |
| Open-Meteo, API histórica | ERA5 y ERA5-Land por coordenada, con agregados diarios | 1940 a la fecha | Sin clave; gratis para uso no comercial hasta 10 mil llamadas por día; CC BY 4.0 | JSON, ligero | Baja | Confirmado por búsqueda; sirve para prototipos, no para la versión final |
| Google Earth Engine, ERA5-Land diario | Agregados diarios listos, extracción por polígono | 1950 a la fecha | Cuenta de Google Cloud; gratis solo para usuarios elegibles (académicos, gobierno para investigación), sujeto a revisión | Sin descarga local | Baja a media | Elegibilidad del Banco por confirmar; no se recomienda como fuente principal |
| SMN, estaciones climatológicas | Precipitación, evaporación, temperatura máxima y mínima diarias de más de cinco mil estaciones | Desde el inicio de cada estación | Gratis, sin registro; un archivo de texto por estación | Texto de ancho fijo; cientos de MB en total | Media: raspado de cinco mil archivos y control de calidad | Confirmado por búsqueda; se usa para validar ERA5 |
| Monitor de Sequía de México (CONAGUA) | Categorías de sequía por municipio y porcentaje de área afectada | Mensual de 2003 a 2014; quincenal desde febrero de 2014 | Gratis; Excel municipal en la página; capas geográficas por correo | Excel, ligero | Baja a media: empatar claves municipales con INEGI | Confirmado por búsqueda; robustez del índice de sequía |
| CONAGUA SINA, monitoreo de presas | Almacenamiento diario de 210 presas, 181 principales | Desde 2007, diario | Gratis, sin registro | Excel, PDF, capas | Media: probablemente hay que raspar la consulta; descarga completa por confirmar | Servidor con caídas ocasionales |
| NOAA HURDAT2 e IBTrACS | Trayectorias de ciclones con posición, viento, presión y radios de viento cada seis o tres horas; IBTrACS cubre Atlántico y Pacífico en un archivo | 1851 a la fecha (Atlántico), 1949 (Pacífico) | Gratis, sin registro | CSV, NetCDF, shapefile; menos de 10 MB | Baja | Confirmado por búsqueda; IBTrACS es la fuente principal |

**B. Energía en México**

| Fuente | Contenido | Periodo y frecuencia | Acceso y costo | Formato y volumen | Complejidad | Estado |
|---|---|---|---|---|---|---|
| CENACE, Área Pública del SIM: estimación de la demanda real | Demanda horaria por sistema (SIN, BCA, BCS) y por gerencia de control regional, por día operativo y liquidación | Desde 2016 (por confirmar), horario | Gratis, sin registro | CSV por día; decenas de MB por año | Media: muchos archivos, cambios de formato y de horario de verano | Confirmado por búsqueda |
| CENACE, SIM: energía generada por tipo de tecnología | Generación por tecnología (hidro, ciclo combinado, térmica convencional, carbón, nuclear, geotermia, eólica, solar) por sistema y mes operativo | Desde 2016, granularidad horaria por confirmar | Gratis, sin registro | CSV, ligero | Baja a media | Confirmado por búsqueda |
| CENACE, SIM: precios marginales locales (MDA y MTR) | PML horario por nodo (cerca de 2,400) y por nodos distribuidos, con componentes de energía, congestión y pérdidas | Desde enero de 2016, horario | Gratis, sin registro; servicio web público con tope de siete días y 20 nodos por llamada | CSV; cerca de 1 GB por año a nivel nodo; ligero para nodos distribuidos | Media a alta a nivel nodo; baja con nodos distribuidos | Confirmado por búsqueda; parte de la serie migró a datos.gob.mx en 2021 |
| SENER, Sistema de Información Energética | Producción, importación, exportación y ventas de petrolíferos por producto; producción e importación de gas natural por ducto y GNL; generación por tecnología y consumo de combustibles para generación | Mensual, la mayoría desde los años noventa | Gratis; cuadros con exportación a Excel; sin API documentada | Excel por cuadro, ligero | Baja a media: muchos cuadros, cortes de serie | Mecánica de exportación por confirmar |
| Pemex, Base de Datos Institucional | Producción, proceso de crudo por refinería, elaboración de petrolíferos, importaciones y exportaciones por producto, ventas por producto y entidad, precios | Mensual desde 1990; preliminar en la última semana del mes siguiente | Gratis, sin registro | Excel o CSV por cuadro, ligero | Baja | Confirmado por búsqueda |
| CNE (antes CRE), precios de gasolinas y diésel | Precios por estación (seis cortes diarios) en consulta en vivo; datos abiertos con promedios diarios nacionales y mensuales por entidad, histórico de precios reportados por permisionarios y volúmenes vendidos por permisionario | Desde 2017 | Gratis, sin registro | Excel, XML, CSV; el histórico por estación pesa varios GB si se despliega | Baja para promedios por entidad; media a alta por estación | Si existe un archivo único del histórico diario por estación está por confirmar; respaldar el histórico al inicio por el cambio de CRE a CNE |
| Profeco, Quién es Quién en los Combustibles | Reportes semanales por ciudad y marca | Semanal | Gratis | PDF | Baja | Solo para narrativa |
| CNE, Índice de Referencia Nacional de Precios de Gas Natural al Mayoreo | Precio promedio ponderado nacional y regional en pesos y dólares por gigajoule, y volumen | Mensual desde julio de 2017 | Gratis | Excel | Baja | Último mes confirmado: julio de 2025; publicación en 2026 por confirmar |
| SHCP, acuerdos semanales del estímulo al IEPS (DOF) | Porcentajes, montos del estímulo y cuotas disminuidas por combustible; desde 2022, estímulo complementario | Semanal desde 2017, cerca de 500 acuerdos | Gratis | HTML del DOF, una página por acuerdo | Media: no se encontró tabla consolidada de Hacienda; hay que raspar el DOF; las compilaciones del CIEP sirven para cotejar | Tabla consolidada por confirmar; la captura semanal actual ya existe en el pipeline del reporte semanal |
| SHCP, Estadísticas Oportunas de Finanzas Públicas | Recaudación mensual del IEPS de gasolinas y diésel por concepto, negativa en meses de 2022 | Mensual desde 1990 | Gratis | Excel desde la consulta interactiva | Baja | Exportación por confirmar |
| Terminal financiera del Banco | Diferenciales de gasolina y diésel frente al crudo en la costa del Golfo, precios de gas en centros de Texas, curva de futuros | Diario | Ya contratada | Exportación a Excel | Baja | Disponible |

**C. Estados Unidos y canal externo**

| Fuente | Contenido | Periodo y frecuencia | Acceso y costo | Formato y volumen | Complejidad | Estado |
|---|---|---|---|---|---|---|
| EIA, API versión 2 | Entradas y utilización de refinerías del distrito 3, inventarios semanales, precios spot de gasolina (desde 1986) y diésel de bajo azufre (desde 2006) en la costa del Golfo, exportaciones mensuales a México por producto, exportaciones de gas por ducto a México | Semanal, diario y mensual | Clave gratuita por correo; tope de 5 mil filas por llamada | JSON o CSV, ligero | Baja | Confirmado por búsqueda |
| EIA, análisis de huracanes | Artículos sobre Harvey (2017), Ida (2021) y perspectiva del STEO de 2023 sobre paros por huracanes; para Beryl (2024) no se encontró artículo específico | Por evento | Gratis | HTML | Baja | Confirmado por búsqueda |
| Paros de refinerías | No hay base pública; los proveedores son de pago (servicios de información especializada). Sustitutos gratuitos: reportes de eventos de emisiones de la agencia ambiental de Texas, estadísticas de cierre de plataformas de la agencia federal de seguridad costa afuera, reportes de situación del Departamento de Energía durante tormentas | Por evento | Gratis los sustitutos | HTML, PDF | Media a alta para construir una lista de eventos | Se recomienda usar la utilización semanal del distrito 3 como medida agregada del paro |

### 4.3 Qué se obtiene sin pedir nada y qué convendría pedir

Sin pedir: todo el inventario anterior. La única fuente de pago que aparece (bases de paros de refinerías) no es necesaria; la utilización semanal del distrito 3 y los reportes por evento la sustituyen.

Convendría pedir, sin que el proyecto dependa de ello:

- A DME, su base de eventos extremos, para comparar definiciones y usarla como robustez.
- A la CFE o a la CRE, nada: el costo de combustibles para generación no es público con detalle, pero el consumo de combustibles por tecnología está en el Sistema de Información Energética y los precios en la terminal, lo que permite construirlo.

### 4.4 Construcción de la base

1. **Clima.** Descargar de ERA5 las estadísticas diarias de temperatura máxima y mínima y de precipitación para la caja de México de 1991 a 2025 (para la climatología, alrededor de 3 a 6 GB) y, si se quiere la serie larga, de 1940 a 1990 en un segundo paso. Descargar además la serie horaria por punto para una ciudad de referencia por región de control. Ponderar la malla a regiones de control con población del marco geoestadístico del INEGI.
2. **Eventos.** Calcular umbrales por percentil y los índices de sequía SPI y SPEI por región y por cuenca de las presas hidroeléctricas principales (Grijalva, Balsas, Santiago y Fuerte). Empalmar con el Monitor de Sequía y con el almacenamiento de presas para validar.
3. **Ciclones.** Procesar IBTrACS para el Atlántico y el Pacífico; asignar municipios dentro de los radios de viento; identificar los que tocan tierra en Texas y Luisiana.
4. **Mercado eléctrico.** Descargar del SIM la demanda real por región de control para todos los días desde 2016, la generación por tecnología y los precios marginales de nodos distribuidos. Documentar los cambios de formato y de liquidación.
5. **Hidrocarburos.** Exportar los cuadros mensuales del SIE y de la BDI; descargar de la EIA por API. Empalmar el índice de gas natural con los precios de Texas de la terminal.
6. **Combustibles y estímulos.** Extender hacia atrás la captura semanal del acuerdo del DOF que ya hace el reporte semanal, con un script sobre las páginas del DOF desde 2017; descargar los promedios de precios por entidad y los volúmenes de la CNE; respaldar todo al inicio.
7. **Documentación.** Un cuaderno por fuente con la descarga, la limpieza y las decisiones, para que la base sea reproducible y se pueda compartir con DME y DASPERI.

Estimación de esfuerzo: entre seis y ocho semanas de una persona para dejar la base completa, con la descarga de ERA5 y el raspado del DOF como los pasos más largos.

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

Las referencias marcadas con asterisco se identificaron por búsqueda y hay que confirmar autores o datos bibliográficos antes de citarlas.

**Temperatura, clima y energía**

- Auffhammer, M. (2018). Climate Adaptive Response Estimation: Short and Long Run Impacts of Climate Change on Residential Electricity and Natural Gas Consumption. NBER Working Paper 24397. Versión publicada en Journal of Environmental Economics and Management (2022).*
- Auffhammer, M., Baylis, P. y Hausman, C. H. (2017). Climate change is projected to have severe impacts on the frequency and intensity of peak electricity demand across the United States. PNAS, 114(8). https://www.pnas.org/doi/abs/10.1073/pnas.1613193114
- Auffhammer, M. y Mansur, E. T. (2014). Measuring climatic impacts on energy consumption: A review of the empirical literature. Energy Economics, 46.*
- Davis, L. W. y Gertler, P. J. (2015). Contribution of air conditioning adoption to future energy use under global warming. PNAS, 112(19), 5962-5967. https://www.pnas.org/doi/10.1073/pnas.1423558112
- Deschênes, O. y Greenstone, M. (2011). Climate Change, Mortality, and Adaptation: Evidence from Annual Fluctuations in Weather in the US. American Economic Journal: Applied Economics, 3(4), 152-185. https://www.aeaweb.org/articles?id=10.1257/app.3.4.152
- Rode, A., Carleton, T., Delgado, M. y coautores (2021). Estimating a social cost of carbon for global energy consumption. Nature, 598, 308-314. https://www.nature.com/articles/s41586-021-03883-8
- Wenz, L., Levermann, A. y Auffhammer, M. (2017). North-south polarization of European electricity consumption under future warming. PNAS. https://www.pnas.org/doi/full/10.1073/pnas.1704339114
- Temperature Effects on Electricity and Gas Consumption: Empirical Evidence from Mexico and Projections under Future Climate Conditions. Sustainability, 13(1), 305 (2021). https://www.mdpi.com/2071-1050/13/1/305 *
- Domestic electricity consumption in Mexican metropolitan areas under climate change scenarios. Atmósfera (2022). https://www.scielo.org.mx/scielo.php?pid=S0187-62362022000300449&script=sci_arttext&tlng=en *
- How rising temperatures affect electricity consumption and economic development in Mexico. Environment, Development and Sustainability (2024). https://link.springer.com/article/10.1007/s10668-024-04527-3 *

**Huracanes y refinación**

- Congressional Research Service (2005). Oil and Gas Disruption From Hurricanes Katrina and Rita (RL33124) y Oil and Gas: Supply Issues After Katrina and Rita (RS22233). https://www.everycrsreport.com/reports/RL33124.html
- EIA (2017). Hurricane Harvey caused U.S. Gulf Coast refinery runs to drop, gasoline prices to rise. Today in Energy. https://www.eia.gov/todayinenergy/detail.php?id=32852
- EIA (2021). Hurricane Ida disrupted crude oil production and refining activity. Today in Energy. https://www.eia.gov/todayinenergy/detail.php?id=49576
- EIA (2023). How do hurricane-related outages affect gasoline markets. Short-Term Energy Outlook, perspectiva de julio. https://www.eia.gov/outlooks/steo/report/perspectives/2023/07-hurricanes/article.php
- EIA (2007). Refinery Outages: Description and Potential Impact on Petroleum Product Prices. https://www.eia.gov/petroleum/articles/refoutagesindex.php
- Forecast-based disruptions in the energy sector: economic impacts of anticipatory hurricane responses in US Gulf Coast refineries. Environmental Research Letters (2025). https://iopscience.iop.org/article/10.1088/1748-9326/ae0e3a *
- Lewis, M. S. (2009). Temporary Wholesale Gasoline Price Spikes Have Long-Lasting Retail Effects: The Aftermath of Hurricane Rita. Journal of Law and Economics, 52(3).*

**Episodios**

- Argonne National Laboratory (2021). February 2021 Electricity Blackouts and Natural Gas Shortages in Texas (ANL-21/29). https://publications.anl.gov/anlpubs/2021/07/169454.pdf
- Cascading risks: Understanding the 2021 winter blackout in Texas. Energy Research and Social Science (2021). https://www.sciencedirect.com/science/article/pii/S2214629621001997 *
- Cifras de generación hidroeléctrica de la CFE en 2022 y 2023 citadas por prensa; confirmar con CENACE, energía generada por tipo de tecnología.

**Banco de México**

- Arellano-González, J., Juárez-Torres, M. y Zazueta-Borboa, F. (2023). Weather shocks, prices and productivity: Evidence from staples in Mexico. Documento de Investigación 2023-16, Banco de México.
- Banco de México, PNUMA y PNUD (2020). Riesgos y oportunidades climáticas y ambientales del sistema financiero de México: del diagnóstico a la acción.
- Banco de México. Reporte sobre las Economías Regionales, recuadro sobre la opinión empresarial acerca del impacto de eventos climáticos.
- Programa de Trabajo DGIE 2026-2027, proyecto 10, entregables ii y iii (DME).

**Fuentes de datos (direcciones)**

- ERA5: https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels ; estadísticas diarias: https://cds.climate.copernicus.eu/datasets/derived-era5-single-levels-daily-statistics ; series por punto: https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels-timeseries ; API: https://cds.climate.copernicus.eu/how-to-api
- Open-Meteo: https://open-meteo.com/en/docs/historical-weather-api
- SMN estaciones: https://smn.conagua.gob.mx/es/climatologia/informacion-climatologica/informacion-estadistica-climatologica
- Monitor de Sequía: https://smn.conagua.gob.mx/es/climatologia/monitor-de-sequia/monitor-de-sequia-en-mexico
- SINA presas: https://sinav30.conagua.gob.mx:8080/Presas/
- IBTrACS: https://www.ncei.noaa.gov/products/international-best-track-archive ; HURDAT2: https://www.nhc.noaa.gov/data/
- CENACE SIM: https://www.cenace.gob.mx/APSIM.aspx ; demanda real: https://www.cenace.gob.mx/Paginas/SIM/Reportes/EstimacionDemandaReal.aspx ; generación por tecnología: https://www.cenace.gob.mx/Paginas/SIM/Reportes/EnergiaGeneradaTipoTec.aspx ; PML: https://www.cenace.gob.mx/Paginas/SIM/Reportes/H_PreciosEnergiaSisMEM.aspx
- SIE: https://sie.energia.gob.mx/inicio/
- Pemex BDI: https://ebdi.pemex.com
- CNE precios: https://www.cne.gob.mx/ConsultaPrecios/GasolinasyDiesel/GasolinasyDiesel.html ; datos abiertos: https://www.gob.mx/cne/articulos/consulta-de-datos-abiertos ; volúmenes por permisionario: https://historico.datos.gob.mx/busca/dataset/volumenes-de-petroliferos-reportados-por-permisionarios
- Índice de gas natural: https://www.cne.gob.mx/IPGN/
- DOF, acuerdo semanal (ejemplo): https://dof.gob.mx/nota_detalle.php?codigo=5778057&fecha=09/01/2026
- Estadísticas Oportunas: https://www.finanzaspublicas.hacienda.gob.mx/
- EIA API: https://www.eia.gov/opendata/ ; utilización distrito 3: https://www.eia.gov/dnav/pet/hist/LeafHandler.ashx?n=PET&s=W_NA_YUP_R30_PER&f=W ; exportaciones a México: https://www.eia.gov/dnav/pet/PET_MOVE_EXPCP_A1_NMX_EPP0_EEX_MBBL_M.htm
