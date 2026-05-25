# tp1-eda-delitos-caba-2024
Trabajo práctico de análisis exploratorio de delitos en CABA durante 2024.
# Análisis Exploratorio de Delitos en CABA - 2024

## Objetivo del trabajo

Realizar un proceso de limpieza, análisis exploratorio y visualización de un DataSet de delitos registrados en la Ciudad de Buenos Aires durante el año 2024, identificando patrones relevantes y respondiendo hipótesis planteadas inicialmente.

---

## Contexto del dataset

El DataSet utilizado corresponde a registros públicos de delitos ocurridos en la Ciudad Autónoma de Buenos Aires durante el año 2024.

Los datos incluyen información temporal, geográfica y tipológica de los hechos registrados.

La información fue obtenida desde el portal oficial de datos abiertos del Gobierno de la Ciudad Autónoma de Buenos Aires y contiene variables temporales, geográficas y tipológicas relacionadas con los hechos registrados. 

El análisis fue realizado utilizando el archivo `delitos_2024.csv` obtenido desde el mencionado portal oficial de datos abiertos del Gobierno de la Ciudad Autónoma de Buenos Aires.

Fuente: https://data.buenosaires.gob.ar/dataset/delitos/resource/49f58c2e-21d7-4766-84e0-4bb753d28478

---

## Notebook principal

El desarrollo completo del Análisis Exploratorio de Datos (EDA) se encuentra en el archivo:

`TPN1_Analisis_Delitos_CABA_2024.ipynb`

La notebook incluye:
- carga y limpieza de datos
- análisis exploratorio (EDA)
- visualizaciones estadísticas y geográficas
- análisis de correlaciones
- conclusiones finales

---

## Diccionario de datos del DataSet original 

| Variable | Descripción | Tipo de Dato |
|----------|-------------|--------------|
| id-mapa | Identificador del registro | integer |
| anio | Año del hecho | integer | 
| mes | Mes del hecho | string |
| dia | Día de la semana | string |
| fecha | Fecha del registro | date |
| franja | Franja horaria | integer |
| tipo | Tipo de delito | string |
| subtipo | Subtipo de delito | string |
| uso_arma | Indica uso de arma | string |
| uso_moto | Indica uso de moto | string |
| barrio | Barrio del hecho | string |
| comuna | Comuna correspondiente | number |
| latitud | Coordenada geográfica | geo_point |
| longitud | Coordenada geográfica | geo_point |
| cantidad | Cantidad de registros | number |

---

## Diccionario de datos del DataFrame limpio

| Variable | Descripción | Tipo de Dato |
|----------|-------------|--------------|
| id-mapa | Identificador del registro | integer |
| anio | Año del hecho | integer | 
| mes | Mes del hecho | string |
| dia | Día de la semana | string |
| fecha | Fecha del registro | datetime |
| franja | Franja horaria | float |
| tipo | Tipo de delito | string |
| subtipo | Subtipo de delito | string |
| uso_arma | Indica uso de arma | string |
| uso_moto | Indica uso de moto | string |
| barrio | Barrio del hecho | string |
| comuna | Comuna correspondiente | float |
| latitud | Coordenada geográfica | float |
| longitud | Coordenada geográfica | float |
| cantidad | Cantidad de registros | integer |

---

## Metodología de trabajo aplicada

El análisis fue desarrollado utilizando Python como lenguaje principal, trabajando en Microsoft Visual Studio Code como entorno de desarrollo (IDE) y empleando librerías orientadas al análisis y visualización de datos como Pandas, Matplotlib y Seaborn.

Las principales etapas realizadas fueron:

- Carga y exploración inicial del DataSet
- Conversión y validación de tipos de datos
- Detección y tratamiento de valores nulos e inconsistentes
- Eliminación de registros inválidos
- Generación de estadísticas descriptivas
- Análisis exploratorio mediante histogramas, gráficos de barras, boxplots y mapas de calor
- Evaluación de correlaciones entre variables numéricas
- Identificación de patrones geográficos y temporales
- Elaboración de conclusiones finales a partir de los resultados obtenidos

---

## Conclusiones y hallazgos relevantes

- El análisis exploratorio permitió identificar patrones espaciales y temporales relevantes en los delitos registrados en CABA durante 2024.
- Se observó una concentración significativa de hechos en zonas céntricas y de alta circulación urbana.
- Los delitos de tipo robo y hurto representaron la mayor proporción de registros analizados.
- Las franjas horarias diurnas y vespertinas concentraron la mayor cantidad de hechos reportados.
- Algunos barrios presentaron mayores niveles de concentración delictiva respecto de otros sectores de la Ciudad.
- La limpieza y depuración de datos permitió mejorar la consistencia de las visualizaciones geográficas y reducir registros inválidos.
