# Datos utilizados

## Fuente de datos

Los datos utilizados en este proyecto provienen del portal oficial de **Buenos Aires Data**, correspondiente al dataset **Sistema Único de Atención Ciudadana (SUACI / BA Colaborativa)**, publicado por el Gobierno de la Ciudad Autónoma de Buenos Aires. El conjunto de datos contiene información sobre los contactos y solicitudes realizadas por la ciudadanía, incluyendo fechas, categorías, canales de atención y referencias geográficas. 

**Dataset oficial:**

https://data.buenosaires.gob.ar/dataset/sistema-unico-atencion-ciudadana

---

## Archivos utilizados

Debido al tamaño de los archivos, los datasets originales no se incluyen en este repositorio.

Durante el desarrollo del proyecto se utilizaron los siguientes archivos CSV:

| Archivo | Período |
|----------|---------|
| `sistema-unico-de-atencion-ciudadana-2021.csv` | Año 2021 |
| `sistema-unico-de-atencion-ciudadana-2022.csv` | Año 2022 |
| `sistema-unico-de-atencion-ciudadana-2023.csv` | Año 2023 |

Los tres archivos fueron integrados mediante Power Query para construir una única tabla de hechos utilizada en el modelo dimensional.

---

## Variables principales

Los datasets contienen, entre otras, las siguientes variables de interés:

- Número de solicitud
- Fecha de ingreso
- Fecha de cierre
- Canal de atención
- Categoría
- Tipo de solicitud
- Estado de la solicitud
- Género
- Comuna
- Barrio
- Calle
- Coordenadas geográficas (latitud y longitud)

Estas variables permitieron construir las dimensiones del modelo estrella y desarrollar los indicadores analíticos utilizados en el dashboard.

---

## Procesamiento realizado

Antes del modelado en Power BI se realizaron las siguientes tareas:

- Integración de los archivos correspondientes a los años 2021, 2022 y 2023.
- Limpieza y estandarización de registros.
- Eliminación de valores inconsistentes.
- Construcción de dimensiones mediante Power Query.
- Creación de claves sustitutas (*Surrogate Keys*).
- Implementación de un modelo dimensional (*Star Schema*).

---

## Licencia

Los datos son de acceso público y se encuentran disponibles en el portal oficial de Buenos Aires Data bajo la licencia indicada por el organismo publicador.
