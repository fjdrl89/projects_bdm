# Proyecto 2. Precio efectivo del carbono en los combustibles automotrices en México

Propuesta de entregable 2027 para el proyecto 10 del Programa de Trabajo DGIE 2026-2027 ("Investigación sobre economía ambiental y finanzas sustentables").
Versión 1, 29 de septiembre de 2026. Uso interno.

## 0. Ficha para el PTI

| Campo | Contenido |
|---|---|
| Dirección | [Dirección del proponente] |
| Título | Precio efectivo del carbono en los combustibles automotrices en México |
| Entregable | Nota técnica |
| Trimestre | 2027 T2 (con margen a T3) |
| Línea del proyecto 10 con la que dialoga | Políticas y medidas ambientales (objetivo general); compromisos climáticos (DAI) |

**Párrafo para el PTI (141 palabras):**

> [Dirección] Precio efectivo del carbono en los combustibles automotrices en México. México grava las gasolinas y el diésel con una cuota fija del IEPS y con un impuesto al carbono desde 2014, pero desde 2017 los estímulos fiscales semanales reducen o eliminan esas cuotas cuando suben los precios internacionales. Se construye una serie semanal del precio efectivo del carbono por combustible, neto de estímulos, siguiendo la metodología de tasas efectivas de carbono de la OCDE, y se compara con los instrumentos de otros países, con los umbrales de referencia del FMI y con los impuestos estatales y el sistema de comercio de emisiones de México. Se cuantifica el costo fiscal de los estímulos, su incidencia por decil de ingreso con la ENIGH y su efecto sobre el consumo y las emisiones, con elasticidades estimadas a partir de las ventas estatales de combustibles. Se elaborará una nota técnica. (2027 T2)

## 1. Pregunta y motivación

**Pregunta.** ¿Cuál es el precio del carbono que efectivamente pagan los consumidores de gasolina y diésel en México, semana a semana, y qué implica su volatilidad para la política ambiental, las finanzas públicas y la inflación?

**Por qué importa para el Banco.** Los combustibles automotrices son el eslabón entre la política ambiental y los precios que el Banco sigue de cerca. La cuota del IEPS es el instrumento fiscal más grande sobre las emisiones del transporte en México, muy por encima del impuesto al carbono explícito. Los estímulos semanales son el instrumento con el que Hacienda amortigua los choques de precios internacionales sobre el INPC. Las dos cosas son la misma cuota vista desde dos lados: como señal ambiental y como estabilizador de precios. Medir el precio efectivo del carbono es medir cuánto de la señal ambiental se sacrifica para estabilizar la inflación, y a qué costo fiscal.

**El hueco.** Las mediciones internacionales (OCDE, Banco Mundial, FMI) toman una fotografía anual del impuesto vigente en una fecha. Para México esa fotografía es engañosa: en 2022 la cuota efectiva de las gasolinas fue cero durante meses y el estímulo complementario la volvió negativa. Ninguna fuente pública lleva la serie semanal del precio efectivo del carbono, ni la descompone entre cuota estatutaria, impuesto al carbono y estímulos, ni la traduce a pesos por tonelada de CO2 comparables con otros países.

**Qué aporta.** Una serie semanal desde 2017 del precio efectivo del carbono por combustible, en pesos, dólares y euros por tonelada. Una comparación internacional que sitúa a México frente a la OCDE, a América Latina y a los umbrales de referencia. Una cuenta del costo fiscal de los estímulos contrastada con las cifras oficiales. Y dos extensiones que le dan filo: cuántas emisiones adicionales indujo el estímulo de 2022 y 2023, y quién se benefició por decil de ingreso.

## 2. Relación con el objetivo del proyecto 10 y con las líneas existentes

El objetivo del proyecto 10 empieza por "las políticas y medidas ambientales" y su interacción con la actividad económica. Los entregables actuales miran políticas climáticas de otros países (índice de desempeño climático, compromisos corporativos). Ninguno mira la política de precios al carbono de México. Esta propuesta cubre ese hueco con el instrumento que más pesa: la fiscalidad de los combustibles.

Dialoga con la línea de DAI sobre compromisos climáticos: la OCDE y el FMI usan el precio efectivo del carbono como indicador del entorno de política climática de cada país, comparable al índice de desempeño climático que usa DAI. La serie mexicana podría alimentar esa comparación.

## 3. Antecedentes y literatura

[PENDIENTE: se completa con la verificación de referencias.]

## 4. Datos

[PENDIENTE: inventario de fuentes con condiciones de acceso verificadas.]

## 5. Metodología

### 5.1 Construcción de la serie semanal

Para cada combustible (gasolina menor a 92 octanos, gasolina de 92 octanos o más, diésel) y cada semana desde enero de 2017:

1. **Cuota estatutaria.** Cuota fija del IEPS (artículo 2-A de la Ley del IEPS) vigente en el año, en pesos por litro.
2. **Impuesto al carbono.** Cuota del IEPS a combustibles fósiles (artículo 2, fracción I, inciso H) vigente en el año, en pesos por litro.
3. **Estímulo ordinario.** Porcentaje y monto del estímulo del acuerdo semanal de Hacienda publicado en el Diario Oficial.
4. **Estímulo complementario.** Monto del estímulo complementario (desde marzo de 2022) del acuerdo semanal.
5. **Cuota efectiva.** Suma de 1 y 2 menos 3 y 4, en pesos por litro. Puede ser negativa.
6. **Factor de emisión.** Kilogramos de CO2 por litro de cada combustible, con el factor oficial mexicano y el del IPCC como robustez.
7. **Precio efectivo del carbono.** Cuota efectiva entre factor de emisión, en pesos por tonelada de CO2; se convierte a dólares y euros con el tipo de cambio FIX y el euro del Banco.

Se excluye el IVA, como hace la OCDE, porque grava por igual a todos los bienes. Se documenta la decisión y se reporta una variante con IVA.

### 5.2 Agregación y comparación internacional

La serie por combustible se pondera por las ventas internas de cada uno (SENER) para obtener el precio efectivo del carbono del transporte carretero. Se compara con:

- las tasas efectivas de carbono del transporte carretero de la OCDE para los países miembros y para los latinoamericanos que cubre;
- la tasa efectiva neta de la OCDE, que descuenta subsidios a los combustibles fósiles;
- los umbrales de referencia del FMI para un piso al precio del carbono según nivel de ingreso;
- el precio del sistema de comercio de emisiones de la Unión Europea y el del sistema mexicano, si hay precio observable;
- los impuestos estatales al carbono en México, con la aclaración de que gravan a emisores industriales y no a los combustibles automotrices.

Se muestra que la fotografía anual de las fuentes internacionales coincide con la serie semanal solo en años tranquilos y se aleja en años de precios altos.

### 5.3 Costo fiscal

Costo del estímulo por semana igual a estímulo por litro por ventas del combustible (litros diarios por siete). Las ventas vienen de las series mensuales de SENER interpoladas a semanas y, como robustez, de los datos abiertos de ventas por estación de la CNE. El costo anual se contrasta con tres cifras oficiales: la recaudación mensual del IEPS de gasolinas y diésel de las estadísticas oportunas de Hacienda (negativa en 2022), la estimación del Presupuesto de Gastos Fiscales y los informes trimestrales de finanzas públicas.

### 5.4 Efecto sobre el consumo y las emisiones

Se estima la elasticidad precio de las ventas de gasolina y diésel con un panel de entidades federativas y meses. El precio en estación por entidad viene de los datos abiertos de la CNE; las ventas, de SENER y de la CNE. El instrumento para el precio es el componente del precio internacional de referencia que Hacienda usa para fijar el estímulo, que es exógeno a la demanda estatal. Con la elasticidad se calcula el consumo contrafactual sin estímulo en 2022 y 2023 y las emisiones adicionales inducidas, en toneladas de CO2 y como proporción de las emisiones del transporte del inventario nacional.

### 5.5 Incidencia distributiva

Con la ENIGH 2022 y 2024 se calcula el gasto en gasolina y diésel por decil de ingreso y la proporción del estímulo que capturó cada decil. Es un cálculo directo de incidencia, sin respuestas de comportamiento, con la advertencia correspondiente. Sirve para contrastar el argumento de que el estímulo protege a los hogares de menores ingresos.

### 5.6 Un indicador que se pueda seguir

La serie se diseña para actualizarse cada semana con el acuerdo del Diario Oficial. Puede alimentar el seguimiento del estímulo que ya se hace en el reporte semanal de mercados petroleros y convertirse en un indicador de política ambiental de México para uso interno.

## 6. Resultados esperados

1. Serie semanal 2017-2026 del precio efectivo del carbono por combustible y agregada, en pesos, dólares y euros por tonelada de CO2.
2. Descomposición entre cuota fija, impuesto al carbono, estímulo ordinario y complementario.
3. Posición de México frente a la OCDE, América Latina y los umbrales del FMI, en años tranquilos y en años de precios altos.
4. Costo fiscal anual de los estímulos, con contraste contra las cifras oficiales.
5. Elasticidad precio de la demanda de gasolina y diésel por entidad y emisiones adicionales inducidas por el estímulo.
6. Incidencia del estímulo por decil de ingreso.
7. Un indicador semanal actualizable.

## 7. Entregables y calendario

| Periodo | Actividad | Producto intermedio |
|---|---|---|
| 2026 T4 | Recolección de acuerdos semanales del DOF, cuotas anuales, ventas, precios en estación, factores de emisión, bases OCDE, FMI y Banco Mundial | Serie semanal y documentación |
| 2027 T1 | Comparación internacional, costo fiscal y elasticidades | Cuadros y gráficas |
| 2027 T2 | Incidencia con ENIGH, redacción, seminario interno | Nota técnica |
| 2027 T3 | Margen para comentarios y versión final | Nota técnica final |

Es el proyecto más rápido de los tres: los datos son públicos, están en formatos manejables y parte del trabajo de captura ya existe en el pipeline del reporte semanal.

## 8. Riesgos y mitigación

| Riesgo | Probabilidad | Mitigación |
|---|---|---|
| Recuperar todos los acuerdos semanales del DOF desde 2017 es laborioso | Media | Hacienda publica tablas consolidadas; si no cubren todo, se descargan los acuerdos del DOF con un script |
| Discusión conceptual sobre si la cuota fija del IEPS es un "precio al carbono" | Alta | Adoptar la definición de la OCDE (impuestos específicos a combustibles cuentan como precio efectivo) y reportar la variante con solo el impuesto al carbono explícito |
| Cambio de la CRE a la CNE afecta los datos abiertos de precios | Media | Descargar y respaldar el histórico al inicio |
| Sensibilidad política de mostrar el estímulo como subsidio | Media | Lenguaje neutro; documento de uso interno; contrastar con las propias cifras de Hacienda |

## 9. Sinergias

- DAI: la serie sirve como indicador de política climática de México comparable con los que usa en su línea de compromisos corporativos.
- DASPERI: el capítulo de incidencia y el de elasticidades se conectan con el análisis de precios de energéticos en el INPC.
- Reporte semanal de mercados petroleros: la captura del acuerdo semanal ya se hace; el indicador se agrega al seguimiento sin costo adicional.

## 10. Referencias

[PENDIENTE: se completa con la verificación de referencias.]
