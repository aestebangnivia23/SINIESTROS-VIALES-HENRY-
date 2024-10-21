# Análisis de siniestros viales en la Ciudad Autónoma de Buenos Aires

**ANDRES ESTEBAN GUTIERREZ NIVIA**

## Introducción

Este proyecto se centra en el análisis de datos sobre accidentes de tránsito en la Ciudad Autónoma de Buenos Aires, con el objetivo de proporcionar información crítica para la reducción de víctimas fatales en siniestros viales. El análisis se realiza desde el rol de analista de datos en colaboración con el **Observatorio de Movilidad y Seguridad Vial (OMSV)** de la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires. Los datos analizados abarcan el período de 2016 a 2021.

---

## Estructura del Proyecto

### Contenido del Repositorio

- **DATOS:**
  - `homicidios.xlsx` y `lesiones.xlsx`: Datasets originales.
  - `siniestrosETL.csv`: Datos extraídos y transformados.
  - `siniestroEDA.csv`: Datos limpiados y listos para análisis.
  - `kpi_1.csv`, `kpi_2.csv`, `kpi_3.csv`: Archivos con indicadores clave de desempeño (KPI).

- **NOTEBOOKS:**
  - `ETL.ipynb`: Proceso de Extracción, Transformación y Carga de datos.
  - `EDA.ipynb`: Análisis Exploratorio de Datos.
  - `Visualizaciones.ipynb`: Creación de visualizaciones y KPI.

- **STREAMLIT:**
  - `Presentación.py`: Aplicación web interactiva.
  - `pages/`: Carpetas con páginas específicas.
  - `requirements.txt`: Lista de bibliotecas necesarias.
  - `mapahomicidios.html`, `mapasiniestros.html`: Mapas consultables a través de Streamlit.

- **GITHUB:**
  - `README.md`: Presentación y explicación del proyecto.
  - `REPORTE.md`: Reporte detallado del proyecto.
  - `.gitignore`: Archivo de excepciones para actualizaciones.
  - `Consigna.md`: Descripción original del proyecto.

- **POWER BI:**
  - `Dashboard/`: Carpeta que contiene el Dashboard en formato .pbix, PDF y PNG.
  - `PI2_PowerBi.pbix`: Dashboard interactivo del proyecto.
  - `PI2_PowerBi.pdf`: Dashboard exportado para visualización rápida.

---

## Proceso de Trabajo

El análisis se centra en los archivos de Excel `homicidios.xlsx` y `lesiones.xlsx`, que contienen información sobre accidentes de tránsito en Buenos Aires. El proceso se desarrolla en las siguientes etapas:

### Paso 1: ETL
- Extracción, transformación y carga de datos de `homicidios.xlsx` y `lesiones.xlsx`.
- Unión de datos de víctimas fatales y víctimas con lesiones en un solo DataFrame.

### Paso 2: EDA
- Normalización de tipos de datos y limpieza.
- Visualización y análisis inicial.
- Creación del archivo `siniestrosEDA.csv` para su uso en Streamlit y Power BI.

### Paso 3: Visualizaciones y KPI
- Creación de visualizaciones específicas y cálculo de KPI en `Visualizaciones.ipynb`.
- Generación de archivos `kpi_1.csv`, `kpi_2.csv`, y `kpi_3.csv` para consulta en Streamlit y Power BI.

### Paso 4: Power BI
- Creación de un dashboard interactivo y un informe de análisis.tros.



## Hallazgos y Patrones en los Datos

Durante el análisis de los datos, se destacaron hallazgos importantes:

- **Lesiones**: El 98.9% de los accidentes viales resultan en lesiones leves o graves, mientras que el 1.1% son fatales.
- **Motociclistas**: Presentan una alta probabilidad de sufrir accidentes fatales (2.7% de los accidentes de motociclistas).
- **Peatones**: El 6% de los accidentes resultan en víctimas fatales.
- **Responsabilidad**: Los autos particulares son los principales responsables de accidentes, aunque los transportes de carga, pasajeros y objetos fijos tienen una mayor tasa de fatalidad.
- **Días de mayor riesgo**: Sábados y domingos son días de menos accidentes pero con más fatalidades, especialmente en autopistas y avenidas principales.

---

## Conclusiones

Con base en el análisis, se pueden concluir los siguientes puntos:

- Los accidentes en horarios de madrugada los fines de semana están relacionados con conductores alcoholizados y alta velocidad.
- Diciembre presenta una alta tasa de fatalidad, especialmente en autopistas, debido a la presencia de conductores ocasionales y vehículos en mal estado.
- La mayoría de los accidentes durante el horario laboral resultan en lesiones menores.

---

## Recomendaciones

Se sugieren las siguientes medidas para reducir la tasa de accidentes fatales:

1. **Controles de verificación técnica vehicular**: Aumentar los controles en noviembre, diciembre y enero.
2. **Controles de alcoholemia**: Reforzar los controles los viernes de 21:00 a 7:00 y los sábados de 22:00 a 8:00.
3. **Restricción de vehículos de carga**: Prohibir la circulación en áreas restringidas de lunes a viernes de 7:00 a 10:00 y de 15:00 a 18:00, especialmente en comunas 1, 4 y 9.
4. **Campañas de concientización**: Implementar campañas sobre el uso del casco para motociclistas y ciclistas, con multas por infracciones.
5. **Controles de velocidad**: Aumentar los controles en autopistas y peajes los domingos.
6. **Concientización sobre maniobras peligrosas**: Informar sobre las consecuencias fatales del estacionamiento en doble fila y cambios de carril sin aviso previo.


