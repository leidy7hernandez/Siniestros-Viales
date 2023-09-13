# Presentación del Proyecto de Análisis de Datos para el Observatorio de Movilidad y Seguridad Vial (OMSV)
El Observatorio de Movilidad y Seguridad Vial (OMSV) es un centro de estudios adscrito a la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires. En el contexto de su misión de promover la seguridad vial y reducir las víctimas de siniestros viales en la ciudad, se nos ha encomendado la tarea de llevar a cabo un proyecto de análisis de datos.

## Objetivo del Proyecto
El objetivo principal de este proyecto es generar información valiosa que permita a las autoridades locales tomar medidas efectivas para reducir la cantidad de víctimas fatales en siniestros viales en la Ciudad de Buenos Aires. Este análisis se llevará a cabo utilizando conjuntos de datos proporcionados por el OMSV, que contienen información sobre homicidios y lesiones en siniestros viales ocurridos en la ciudad durante el período comprendido entre 2016 y 2021.

## Fuentes de Datos
Los datos utilizados en este proyecto provienen de dos conjuntos de datos diferentes, cada uno de los cuales consta de dos hojas de datos:
-> Homicidios en Siniestros Viales: Este conjunto de datos incluye información sobre los homicidios ocurridos en siniestros viales en la Ciudad de Buenos Aires durante el período mencionado. Proporciona detalles sobre los hechos en sí, como la fecha, la ubicación y las circunstancias.
-> Lesiones en Siniestros Viales: El segundo conjunto de datos se centra en las lesiones sufridas por las víctimas de siniestros viales en la ciudad. Al igual que el conjunto de datos de homicidios, proporciona información detallada sobre los incidentes, incluyendo la fecha, la ubicación y la gravedad de las lesiones.

## Origen de los Datos
Es importante destacar que los conjuntos de datos utilizados en este proyecto provienen de una fuente confiable y pública, Buenos Aires Data, lo que garantiza la integridad y la transparencia de los datos.

## Metodología del Análisis
El enfoque de este proyecto se basó en el análisis de estos conjuntos de datos para identificar patrones, tendencias y factores que contribuyan a los siniestros viales y sus consecuencias. Este análisis permitirá a las autoridades tomar decisiones informadas y desarrollar estrategias efectivas para mejorar la seguridad vial en la Ciudad de Buenos Aires.

## Introducción
Para llevar a cabo este análisis, se dispuso de un valioso conjunto de datos recopilados durante el período 2016-2021. Estos datos se desglosan en dos categorías fundamentales: homicidios en siniestros viales y lesiones en siniestros viales, y cada una de ellas contiene dos hojas de datos: una dedicada a los hechos y otra a las víctimas involucradas.

Es importante destacar que el acceso a todo el proceso detallado de cada una de las secciones mencionadas a continuación está disponible en el archivo "Code.ipynb". En caso de dificultades en su visualización a través de la plataforma Git, recomendamos su descarga para una revisión más detallada.

1. Limpieza y preparación de los datos.
2. Exploración de datos y análisis descriptivo.
3. Análisis de víctimas.
4. Análisis espacial.
5. Creación de KIPs y métricas clave.
6. Conclusiones y sugerencias

## 1. Limpieza y Preparación de Datos
Se llevó a cabo la limpieza y preparación de los datos. Durante este proceso, se realizaron tareas de identificación y corrección de valores atípicos (Ejem: "SD" es considerado como "Sin Dato"), no hubo necesidad de eliminar datos duplicados o nulos, se eliminó información que no era relevante para el análisis. El objetivo principal fue garantizar que los datos estuvieran en condiciones óptimas para su análisis posterior.

## 2. Exploración de Datos y Análisis Descriptivo
En esta dase se llevó a cabo una serie de acciones clave para comprender en profundidad la información contenida en el conjunto de datos. El análisis se llevó a cabo por separado para homicidios viales y lesiones viales. Cada uno de estos dos conjuntos de datos se sometió a un proceso detallado de exploración y análisis descriptivo para comprender sus características y tendencias específicas. Esto permitió obtener una comprensión más profunda de los factores que influyen en los homicidios viales y las lesiones viales, y proporcionó información valiosa para las medidas de prevención y seguridad en cada uno de estos aspectos de la seguridad vial en la Ciudad Autónoma de Buenos Aires.

### Homicidios Viales

#### Tasa de homicidios viales (número de homicidios viales por año o mes) como un KPI para seguimiento.
En cuanto a los homicidios viales, se realizó el cálculo de la tasa de homicidios viales, que consiste en determinar el número de homicidios viales por año o mes como un indicador clave de rendimiento (KPI) para su seguimiento. La tasa anual de homicidios viales proporciona una visión a largo plazo de la incidencia de estos casos en la Ciudad Autónoma de Buenos Aires durante un año completo. Este enfoque temporal nos permite identificar tendencias y patrones a lo largo de varios años, lo que resulta fundamental para evaluar el impacto de las políticas y medidas de seguridad implementadas a largo plazo en la reducción de la violencia vial en la ciudad.

![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Tasa%20anual%20de%20Homicidios%20Viales.png)

En la gráfica de la tasa anual de homicidios viales, se destaca una reducción significativa a partir del año 2018. Esta disminución puede atribuirse a la implementación del Decreto 101-2018 por parte del Gobierno de Buenos Aires, que autorizó programas de educación vial. A partir de 2019, se implementó a totalidad el 5954 decto 101-2018 y se llevaron a cabo campañas de concientización destinadas a educar a conductores, peatones y ciclistas, segmentadas por grupos de edad, sobre la importancia de respetar las normas de tráfico y las medidas de seguridad.

Estas campañas de concientización incluyeron charlas educativas en las escuelas y actividades de sensibilización pública. Además, se considera esencial estimar la tasa de homicidios viales a nivel mensual, ya que permite un seguimiento más detallado de la evolución de estos eventos en el corto plazo y facilita la identificación de problemas emergentes.

* Para obtener información adicional sobre estas campañas de educación vial, se puede consultar el siguiente enlace: [Enlace a la información.](https://buenosaires.gob.ar/movilidad/plan-de-seguridad-vial/educacion-para-la-movilidad-sustentable#:~:text=Docentes%3A%201%20Curso%20Educaci%C3%B3n%20Vial%20para%20la%20Movilidad,...%208%20Mi%20primera%20licencia%20...%20M%C3%A1s%20elementos)

![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Tasa%20mensual%20de%20Homicidios%20Viales.png)

El análisis mediante el uso del promedio móvil nos proporciona una perspectiva valiosa sobre la tendencia de la tasa de homicidios viales a lo largo del tiempo. A pesar de un repunte registrado en diciembre de 2020, es evidente que, en general, la tasa ha experimentado una disminución desde la implementación del Decreto 101-2018 (conocido como 5954 decto 101-2018).

Sin embargo, es importante señalar que estos repuntes eventuales en la tasa indican la presencia de desafíos continuos en la solución planteada. Esto subraya la necesidad de seguir profundizando en nuestro análisis y de identificar posibles áreas de mejora para abordar de manera efectiva la problemática de los homicidios viales en la Ciudad de Buenos Aires.

#### Análisis de la distribución de la hora en que ocurren los homicidios viales.
El análisis del momento en que ocurren con mayor frecuencia los homicidios viales es fundamental para tomar decisiones efectivas en cuanto a medidas de seguridad pública. Esta información proporciona insights valiosos que pueden ser utilizados por las autoridades para mejorar la seguridad vial en momentos críticos. Por ejemplo, si se identifica que la mayoría de los homicidios viales ocurren en las primeras horas de la mañana, se pueden diseñar estrategias específicas, como la implementación de patrullas adicionales o campañas de concientización dirigidas a esa franja horaria, con el objetivo de reducir el riesgo y aumentar la seguridad de los ciudadanos.

![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Distribucion%20de%20Homicidios%20Viales%20por%20hora%20del%20dia.png)

El análisis de la distribución horaria de los homicidios viales revela patrones interesantes. En la gráfica, podemos observar que las horas con menor ocurrencia de homicidios viales son las 2:00 AM y la 1:00 PM. Esto puede explicarse por el hecho de que, en esas horas, la mayoría de las personas tiende a no estar en movimiento, ya sea debido al descanso nocturno o a la hora del almuerzo. Por otro lado, las horas con mayor incidencia de homicidios viales son las 6:00 AM y las 7:00 AM. Esta tendencia podría relacionarse con la fatiga o somnolencia de los conductores en las primeras horas de la mañana, ya que es un momento en el que es posible que no hayan tenido suficiente descanso. Estos hallazgos proporcionan información valiosa para la planificación de estrategias de seguridad vial específicas para las horas de mayor riesgo.

#### Exploración de la ubicación de los homicidios en función de la comuna y el tipo de calle.
La consideración del tipo de calle en la que ocurren más homicidios viales es fundamental, ya que esto puede indicar deficiencias en la infraestructura vial que deben abordarse para mejorar la seguridad de los actores viales. Por lo tanto, se genera un gráfico de distribución para identificar las infraestructuras viales más peligrosas para los ciudadanos.

![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Homicidios%20Viales%20por%20Comuna%20y%20Tipo%20de%20Calle.png)

Es interesante notar que la mayoría de los homicidios viales ocurren en las avenidas, lo que tiene sentido debido a varios factores. En primer lugar, las avenidas generalmente tienen un alto flujo de tráfico en comparación con otros tipos de calles. Además, las avenidas son una característica común en la ciudad, lo que aumenta las posibilidades de que ocurran accidentes de tráfico, incluidos los homicidios viales. Es notable que en casi todas las comunas (excepto la comuna 12) se registre un alto número de homicidios viales en las avenidas, lo que sugiere la necesidad de revisar la calidad de estas vías o aumentar la supervisión vial en esas áreas de la ciudad.

Por otro lado, el gráfico revela que la Comuna 1 es la que presenta la mayor cantidad de homicidios viales. Esta comuna es una de las áreas más transitadas y turísticas de Buenos Aires, con una gran cantidad de actividades culturales, comerciales y turísticas. Cada uno de sus barrios tiene su propio carácter y atractivo, lo que la convierte en una parte significativa de la vida urbana en la ciudad.

### Lesiones

#### Análisis de la distribución de la hora y el día de la semana en que ocurren las lesiones viales.
![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Distribucion%20de%20Lesiones%20Viales%20por%20Hora%20del%20Dia.png)

En contraste con los homicidios, las lesiones viales tienden a aumentar alrededor de las 5:00 PM, lo cual se alinea con informes recientes que indican que las horas pico en Buenos Aires comienzan a la 1:00 PM y se extienden hasta las 5:00 PM. Como se refleja en nuestro gráfico, estas son las horas en las que se registran la mayoría de las lesiones viales. Esto sugiere una relación directa entre el flujo de vehículos y la incidencia de lesiones viales, ya que un mayor flujo de tráfico durante las horas pico puede aumentar el riesgo de accidentes.

Fuente: [Enlace a la fuente](https://www.lanacion.com.ar/buenos-aires/fin-de-la-hora-pico-cuales-son-los-horarios-con-mayor-circulacion-de-vehiculos-en-las-autopistas-y-nid04092023/)

Adicionalmente, considerar en qué días de la semana se producen con mayor frecuencia las lesiones viales es crucial para implementar medidas de seguridad dirigidas a proteger a los actores viales que son más activos durante esos días. Esto podría incluir campañas de concientización específicas o patrullas de seguridad adicionales en momentos de mayor riesgo.

![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Distribucion%20de%20Lesiones%20Viales%20por%20D%C3%ADa%20de%20la%20Semana.png)

La gráfica es contundente, sin embargo, es relevante destacar que los accidentes de tráfico y las lesiones viales son eventos multifactoriales, y aunque los viernes pueden experimentar un aumento debido al inicio del fin de semana y las actividades sociales, en términos generales, las lesiones tienden a ocurrir principalmente en los días laborales debido a la mayor actividad relacionada con el trabajo y el tráfico durante estos días. Esto subraya la importancia de implementar medidas de seguridad consistentes a lo largo de la semana para proteger a los actores viales en todo momento.

#### Exploración de la distribución por tipo de vehículo involucrado.

![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Distribucion%20por%20Tipo%20de%20Vehiculo%20Involucrado%20en%20Lesiones%20Viales.png)

Es evidente que la mayoría de las lesiones viales ocurren en motocicletas, y esto puede atribuirse a varias razones. Las motocicletas son vehículos altamente maniobrables, lo que las hace propensas a moverse con agilidad entre el tráfico. Sin embargo, si no se manejan con precaución, esta ventaja puede convertirse en un riesgo, ya que aumenta la posibilidad de colisiones y caídas. Además, algunos motociclistas pueden adoptar comportamientos de conducción riesgosos, como el exceso de velocidad o la omisión del uso de cascos protectores, lo que incrementa aún más el peligro de accidentes y lesiones.

Es crucial destacar la importancia de que los motociclistas respeten los límites de velocidad y sigan las normas de tráfico para mantener la seguridad vial. Esto puede lograrse mediante el uso de cámaras o detectores de velocidad en zonas estratégicas, como las avenidas, así como a través de programas de capacitación en seguridad vial específicamente diseñados para motociclistas. Estas medidas son fundamentales para reducir el número de lesiones viales en motocicletas y proteger la vida de los actores viales.

## 3. Análisis de Víctimas
Uno de los objetivos clave de esta fase fue calcular las posibles relaciones y distribuciones de homicidios y lesiones viales en la Ciudad Autónoma de Buenos Aires. Esta métrica fundamental nos proporcionó información sobre la gravedad de los siniestros viales en la región y fue esencial para comprender la magnitud del problema.

### Análisis de la distribución de edades y sexos de las víctimas en ambos conjuntos de datos.
![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Distribucion%20de%20Edades%20y%20Sexo%20en%20Homicidios%20y%20Lesiones%20Viales.png)

Los datos sobre sexo y edad de las víctimas son fundamentales para desarrollar políticas públicas y medidas de seguridad efectivas. Por ejemplo, en este gráfico se observa que un grupo demográfico particular (jóvenes adultos de entre 20 y 40 años) tiene una alta probabilidad de ser víctima de un accidente de tráfico, tanto hombres como mujeres. Esto sugiere la necesidad de implementar programas de educación vial específicos y campañas de concientización dirigidas a este grupo de edad para promover comportamientos seguros en la vía pública y reducir el riesgo de lesiones viales. Estos datos son valiosos para diseñar estrategias de prevención y mejorar la seguridad vial en la Ciudad Autónoma de Buenos Aires.

### Relación entre la gravedad de las lesiones y el tipo de actor vial
Los resultados de este tipo de estudio pueden tener un impacto significativo en las políticas y regulaciones de tráfico. Por ejemplo, si se encuentra que un cierto tipo de actor vial tiene una mayor probabilidad de sufrir lesiones graves, las autoridades pueden considerar la implementación de restricciones o regulaciones adicionales para mejorar su seguridad. En este análisis, también se tendrán en cuenta los "SD" para obtener una imagen más completa de las lesiones. Se utilizará la Prueba de Chi Cuadrado para determinar si existe una asociación significativa entre la gravedad de las lesiones y el tipo de actor vial, como peatones, ciclistas, conductores de automóviles, etc. Si se encuentra una asociación significativa, esto indicará que el tipo de actor vial y la gravedad de las lesiones no son independientes, lo que proporciona información valiosa para la toma de decisiones en materia de seguridad vial.

![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Distribucion%20Esperada%20de%20Gravedad%20de%20Lesiones%20por%20Tipo%20de%20Actor%20Vial.png)


El análisis de este gráfico revela varias conclusiones importantes. En primer lugar, se destaca la necesidad de mejorar la recopilación de datos sobre accidentes de tránsito en la ciudad de Buenos Aires. La presencia de una cantidad significativa de casos etiquetados como "Sin Datos" sugiere que hay margen para fortalecer las entidades encargadas de la recopilación de datos, ya que contar con información completa y precisa es fundamental para realizar análisis efectivos y tomar medidas de seguridad vial adecuadas.

Además, es preocupante observar que los motociclistas representan el grupo con la mayor cantidad de lesiones graves, y esta diferencia es significativa en comparación con la distribución de lesiones entre automovilistas y ciclistas. Esto resalta la importancia de dirigir esfuerzos hacia la capacitación y concienciación de los motociclistas, así como de aplicar sanciones más rigurosas para aquellos que no cumplan con las normas de seguridad vial, especialmente en lo que respecta al uso de elementos de protección.

Estas conclusiones subrayan la necesidad de implementar políticas y medidas específicas para abordar la seguridad vial de los motociclistas y mejorar la calidad de los datos recopilados en futuros estudios.

## 4. Análisis Espacial
### Localización de áreas geográficas con una alta incidencia de siniestros viales y posiblemente de víctimas fatales.
La identificación de las ubicaciones donde ocurre la mayoría de los siniestros viales es esencial para una asignación eficiente de recursos por parte de las autoridades. Esto les permite concentrar sus esfuerzos y recursos, como oficiales de tráfico, ambulancias y servicios de emergencia, en las áreas de mayor riesgo. Como resultado, se puede proporcionar una respuesta más rápida y efectiva en caso de accidentes, lo que puede marcar la diferencia en la atención a las víctimas y la prevención de lesiones graves o fatales. Esta estrategia contribuye a mejorar la seguridad vial y a reducir el impacto de los siniestros viales en la comunidad.

![Image text](https://github.com/leidy7hernandez/Siniestros-Viales/blob/d48e2d3ae80a5e504060f7fec08bcde26afc252e/Imagenes/Mapa_homicidios_viales.png)

El mapa resalta la importancia de tomar medidas específicas en la Avenida General Paz debido a la alta tasa de siniestros viales en esa área. Para abordar esta problemática, se sugiere la instalación de cámaras de control de velocidad a lo largo de la avenida. Estas cámaras pueden ayudar a monitorear el cumplimiento de los límites de velocidad y detectar conductas de conducción peligrosas. Además, se recomienda aumentar la presencia policial en la zona para mejorar la supervisión y la aplicación de las normas de tráfico. Estas acciones combinadas pueden contribuir significativamente a reducir la incidencia de siniestros viales y a mejorar la seguridad en la Avenida General Paz y sus alrededores.

## 5. Creación de KPIs y Métricas Clave
Se llevaron a cabo la creación de Indicadores Clave de Desempeño (KPIs) y métricas relevantes. Estos indicadores proporcionaron una medición cuantitativa del impacto de las intervenciones y sirvieron como base para la toma de decisiones informadas.

### El Ministerio de Seguridad de la Nación se propuso reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior.
### poblacion_semestral 1 ###
La variación porcentual de la tasa de homicidios viales disminuyó considerablemente en el último semestre analizado, presentando una reducción del -24.02% (la tasa pasó de 1.79 a 1.36). Si bien esto indica que se ha logrado un avance significativo al reducir esta tasa y acercarse al objetivo, es importante destacar que aún es necesario continuar trabajando para mejorar la cifra de fallecidos en siniestros viales. Recordemos que detrás de cada número estadístico hay vidas humanas y familias afectadas, en este caso, 42 familias que han sufrido pérdidas.

### Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior
Este objetivo es de suma importancia, dado que casi la mitad de las víctimas fatales de los siniestros viales son motociclistas.
### poblacion_anual 1 ###
En el año 2021, se observó un incremento en la tasa de homicidios viales en motociclistas del 19.77%, con la tasa anual pasando de 0.94 a 1.49. Como recomendación para alcanzar este objetivo, que ha sido mencionado previamente, se pueden llevar a cabo programas de concientización vial dirigidos específicamente a los motociclistas, además de intensificar la supervisión del uso de equipos de seguridad, como el casco.

### Reducir la tasa anual de homicidios viales en las avenidas en un 20% con respecto al año anterior.
Este objetivo se establece en función de la sección 2, ya que al explorar la ubicación de los homicidios en relación con la comuna y el tipo de calle, se identificó que las avenidas son los lugares donde ocurren con mayor frecuencia los siniestros viales fatales.
### poblacion_anual 2 ###
En los últimos años, la tasa de homicidios viales en las avenidas ha experimentado fluctuaciones significativas, y lamentablemente, no se logró cumplir con el objetivo el año pasado. Sin embargo, con un aumento en la presencia de las autoridades viales en las avenidas, se espera reducir esta tasa de manera efectiva.

## 6. Conclusiones y sugerencias
Este proyecto de análisis de datos fue un esfuerzo destinado a contribuir a la seguridad vial en la Ciudad de Buenos Aires. Los resultados obtenidos en este análisis servirán como base para la implementación de políticas y acciones concretas que ayuden a reducir la cantidad de víctimas fatales en siniestros viales, priorizando la seguridad y el bienestar de los habitantes de la ciudad. A continuación, se presentan las sugerencias derivadas de este análisis:

* Continuar con las capacitaciones implementadas bajo el Decreto 5954/18, específicamente aquellas segmentadas por edades. Se recomienda que estas capacitaciones sean periódicas, al menos una vez al año para toda la comunidad.
* Extender las capacitaciones para incluir consejos sobre la importancia del descanso adecuado para todos los actores viales, con el objetivo de reducir los siniestros viales causados por la somnolencia, especialmente en las primeras horas del día.
* Aumentar la presencia de policía de tránsito en la Comuna 1, la cual es la más concurrida y donde se registran más siniestros viales.
* Destinar mayor inversión en la infraestructura de las avenidas en todas las comunas para mejorar la seguridad vial.
* Reforzar la presencia de autoridades viales durante las horas pico para garantizar un flujo de tráfico seguro y eficiente.
* Implementar cámaras de control de velocidad y detectores en zonas estratégicas para controlar el cumplimiento de las normas de tráfico.
* Ofrecer capacitaciones en seguridad vial específicamente dirigidas a motociclistas y aumentar la supervisión del uso de cascos de seguridad, considerando la posibilidad de aplicar multas en caso de incumplimiento.
* Fortalecer las entidades encargadas de la recopilación de datos relacionados con siniestros viales o crear un grupo de estadistas especializados en este tipo de casos.
* Mantener una vigilancia constante sobre el comportamiento de los conductores en la Avenida General Paz, donde se registra una alta incidencia de siniestros viales.
