![Pandas](https://img.shields.io/badge/-Pandas-333333?style=flat&logo=pandas)
![Numpy](https://img.shields.io/badge/-Numpy-333333?style=flat&logo=numpy)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-333333?style=flat&logo=matplotlib)
![Seaborn](https://img.shields.io/badge/-Seaborn-333333?style=flat&logo=seaborn)
![Python](https://img.shields.io/badge/-Python-333333?style=flat&logo=python)

<h1 align='center'>
 <b>Presentación de Homicidios por Siniestros Viales en la ciudad de Buenos Aires</b>
</h1>

# <h1 align="center">**`PI02_Siniestros_Viales`**</h1>

<h1 align='center'>
 <b>Análisis de Accidentes de Tránsito en la Ciudad de Buenos Aires</b>
</h1>

<p align='center'>
<img src="https://ahorraseguros.mx/wp-content/uploads/2022/12/siniestro.jpg" alt="Accidente de tránsito">
</p>

# Introducción

Este proyecto tiene como objetivo la elaboración de un análisis de datos simulando el rol de un *Data Analyst*, con el fin de generar información que permita tomar medidas para disminuir la cantidad de victimas fatales, para ello, nos proporcionan un dataset sobre homicidios de siniestros viales acontecidos en la Ciudad de Buenos Aires durante el  periodo 2016-2021. Esta información es obtenida gracias al `Observatorio de Movilidad y Seguridad Vial (OMSV)` de la ***Secretaría de Transporte***

# Estructura del Proyecto

### Contenido del Repositorio

- **DATOS**:
  - `homicidios.xlsx` y `lesiones.xlsx`: Datasets originales.
  - `hechos.csv`, `poblacion_comunas.csv`, `victimas.csv`: Datos listos para su consumo externo.
  

- **NOTEBOOKS**:
  - `ETL.ipynb`: Proceso de Extracción, Transformación y Carga.
  - `EDA.ipynb`: Análisis Exploratorio de Datos.
  - `DashBoard.pbix`: DashBoard en Power By.

# Desarrollo de Trabajo

El análisis se centra en dos bases de datos en archivos Excel: `homicidios.xlsx`, `lesiones.xlsx` en complemento con `poblacion_comunas.csv` que contienen información sobre victimas fatales en accidentes de tránsito, informacion sobre victimas con lesiones más no de gravedad fatal y la poblacion total de cada comuna respectivamente, en la Ciudad de Buenos Aires, Argentina. Estos datos se someten a un proceso de ETL para unificar y limpiar los datos, es de resaltar que el rol de este proyecto es un ***Data Analyst***, por lo que no es adecuado realizar transformaciones, ya que no es una función del rol. Luego, se realiza un análisis exploratorio de
datos (EDA) para hallar tendencias, valores duplicados y atípicos, así mismo como patrones en los datos.

### Paso 1: ETL

- Lectura, normalización y limpieza de datos para los archivos `homicidios.xlsx` y `lesiones.xlsx`,
para `poblacion_comuna.csv`no se realizan trabajos adicionales de limpieza ya que provienen estructurados 
correctamente.
- Unión de datos de víctimas fatales y víctimas con lesiones en un solo DataFrame para una mayor agilidad en su análisis exploratorio posterior.

### Paso 2: EDA

- Visualización de dataframes.
- Análisis descriptivo general.
- Determinación de valores duplicados, hallazgo de valores atípicos y búsqueda de distribuciones y patrones de datos.

### Paso 3: Visualizaciones y KPI

- Se crean dos KPIs a partir de las siguientes fórmulas y objetivos a tratar:

- Definio a la tasa de homicidios en siniestros viales como el número de víctimas fatales en 
-    accidentes de tránsito por cada 100,000 habitantes en un área geográfica durante un período de 
-    tiempo específico. Su fórmula es:
-    (Número de homicidios en siniestros viales / Población total) * 100,000
- *Objetivo:* Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses,
-    en la ciudad de Buenos Aires, en comparación con la tasa de homicidios en siniestros viales del semestre anterior.
- Defino a la cantidad de accidentes mortales de motociclistas en siniestros viales como el 
-    número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban 
-    en moto en un determinado periodo temporal. La fórmula para medir la evolución de los 
-    accidentes mortales con víctimas en moto es: 
-    (Número de accidentes mortales con víctimas en moto en el año anterior - Número de accidentes 
-    mortales con víctimas en moto en el año actual) / (Número de accidentes mortales con víctimas 
-    en moto en el año anterior) * 100
- *Objetivo:* Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, 
-    en la ciudad de Buenos Aires, respecto al año anterior.


### Paso 4: Power BI

- Creación de un dashboard interactivo y un informe de análisis(README).

********************************************************************


# Hallazgos y Patrones en los Datos

Durante el análisis de los datos, se destacaron hallazgos importantes:

- Observando y analizando los accidentes fatales totales, es posible destacar que la reducción de homicidios del 10% como objetivo del KPI no se cumple para los años 2016, 2018 y 2020, por lo que no es posible confirmar que las medidas tomadas hasta ahora para la reducción de accidentes sean consistentes con el paso de los años.
- Es importante tener en cuenta que el año 2020 es donde presenta menor cantidad de accidentes y su vez, menos cantidad de datos, que se debe al confinamiento presentado a nivel mundial debido a el COVID-19.
- Se obsevó ademas que el tipo de calle *Avenida* es la que presenta la mayor frecuencia de victimas fatales, esto es un indicativo fuerte para pensar que las avenidad de la ciudad de Buenos Aires pueden presentar fallas tales como la mala información vial o tambien un deterioro de las avenidas que induce a un potencial accidente.

- Mediante el KPI de accidentes en moto que tiene como objetivo disminuir en un 7% las victimas, se puede concluir que sólo el año 2021 no cumplió con el objetivo, donde tambien es posible ver que se una tendencia bajista, esto indica que las medidas tomadas estaban dando resultados postivos hasta el último año que se tuvo registro. Esto proporciona el reto de adoptar nuevas medidas para que la tasa de muertes en moto no aumente para los años próximos.


***

### Enlaces :

* [Repositorio de GitHub](https://github.com/santiagrueda/PI02_Siniestros_Viales_CABA)
* [Linkedin](https://www.linkedin.com/in/santiago-rueda-mira-050b55113/)# PI02_Siniestros_Viales
# PI02_Siniestros_Viales_CABA
