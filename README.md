# Analisis del Sistema Unico de Atencion Ciudadana (SAUC)
> Proyecto desarrollado con Power BI para analizar mas de 3 millones de solicitudes ciudadanas registradas por el Sistema Unico de Atencion Ciudadana (SAUC) de la Ciudad Autonoma de Buenos Aires durante el periodo 2021-2023.

## Introduccion

El presente proyecto tiene como objetivo transformar informacion operativa del Sistema Unico de Atencion Ciudadana (SAUC) en informacion estrategica para la toma de decisiones.

A partir de la integracion y modelado de los datos se construyo un dashboard interactivo que permite monitorear indicadores clave de gestion, analizar la distribucion territorial de las solicitudes y evaluar el uso de los distintos canales de atencion.

Durante el desarrollo se aplicaron tecnicas de ETL, modelado dimensional (Star Schema), Power Query y DAX para optimizar el rendimiento del modelo y facilitar el analisis sobre un volumen superior a **3 millones de registros**.

### ▬ Objetivos del proyecto

* Analizar la evolucion temporal de las solicitudes ciudadanas.
* Medir indicadores clave de gestion (KPIs).
* Identificar las categorias con mayor demanda.
* Analizar la distribucion territorial de las solicitudes.
* Evaluar el nivel de digitalizacion de los canales de atencion.
* Construir un modelo de datos optimizado siguiendo buenas practicas de Business Intelligence.

### ▬ Unidad de analisis

* Solicitudes ciudadanas.
* Categorias.
* Tipos de solicitud.
* Canales de atencion.
* Estado de las solicitudes.
* Distribucion por comuna y barrio.

### ▬ Fuente de datos

- Sistema Unico de Atencion Ciudadana (SAUC)
- Gobierno de la Ciudad Autonoma de Buenos Aires

Periodo analizado:

- 2021
- 2022
- 2023

Cantidad aproximada de registros:

> 3.000.000 de solicitudes.

## Tecnologias utilizadas

- Power BI Desktop
- Power Query
- DAX
- Modelo Estrella (Star Schema)
- Git
- GitHub

## Modelo de datos

El proyecto fue modelado utilizando una arquitectura **Star Schema**, separando la tabla de hechos de las dimensiones para mejorar la organizacion, mantenibilidad y rendimiento del modelo.

### Tabla de hechos

- FactSolicitudes

### Dimensiones

- DimFecha
- DimCanal
- DimCategoria
- DimTipo
- DimEstado
- DimGenero

## ETL

Durante el proceso de preparacion de los datos se realizaron las siguientes transformaciones:

* Integracion de los datasets correspondientes a los años 2021, 2022 y 2023.
* Limpieza y estandarizacion de registros.
* Construccion de dimensiones mediante Power Query.
* Creacion de claves sustitutas (Surrogate Keys).
* Implementacion de un modelo estrella.
* Optimizacion del modelo para consultas analiticas.

## Dashboard

El reporte se organiza en tres paginas principales:

### Resumen Ejecutivo

* Indicadores clave de gestion.
* Evolucion temporal de solicitudes.
* Categorias mas demandadas.
* Estado general de las solicitudes.

### Analisis Territorial

* Distribucion por comuna.
* Distribucion por barrio.
* Analisis geografico de las solicitudes.
* Identificacion de zonas con mayor demanda.

### Canales y Digitalizacion

* Participacion por canal.
* Nivel de digitalizacion.
* Evolucion de los canales digitales.
* Comparacion entre canales de atencion.

## KPIs desarrollados

| Indicador | Descripcion |
|-----------|-------------|
| **Total de Solicitudes** | Cantidad total de solicitudes registradas. |
| **Tasa de Resolucion** | Porcentaje de solicitudes cerradas sobre el total. |
| **Backlog** | Solicitudes pendientes de resolucion. |
| **Nivel de Digitalizacion** | Participacion de los canales digitales sobre el total de solicitudes. |

## Principales resultados

* Identificacion de las categorias con mayor volumen de solicitudes.
* Analisis de la evolucion mensual de la demanda ciudadana.
* Deteccion de diferencias territoriales entre comunas y barrios.
* Evaluacion del crecimiento de los canales digitales.
* Desarrollo de un modelo dimensional optimizado para el analisis de grandes volumenes de informacion.

## Capturas

### Dashboard Ejecutivo

![Dashboard Ejecutivo](images/resumen_ejecutivo.png)

### Analisis Territorial

![Analisis Territorial](images/dashboard_territorial.png)

### Canales y Digitalizacion

![Canales y Digitalizacion](images/dashboard_canales.png)

## Autor

**Mariano Asorey**

Licenciatura en Economia - Universidad de Buenos Aires
