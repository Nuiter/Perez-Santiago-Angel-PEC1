# PEC1 - Análisis Metabolómico

## Descripción del Proyecto
Este repositorio contiene los materiales, código y resultados relacionados con la **PEC1** de metabolómica realizada como parte del curso de bioinformática. El objetivo principal es demostrar la capacidad para analizar un dataset metabolómico utilizando herramientas de R y Bioconductor.

## Estructura del Repositorio

### Archivos Principales

- **`PEC1_Solucion.Rmd`**: Documento principal en formato R Markdown que detalla todos los pasos, análisis y resultados obtenidos.
- **`GastricCancer_NMR.xlsx`**: Dataset utilizado para el análisis.
- **`metabolomics_analysis.Rda`**: Objeto `SummarizedExperiment` que contiene los datos procesados y los metadatos.
- **`stats_table.csv`**: Resultados estadísticos de las pruebas univariantes en formato CSV.
- **`README.md`**: Este archivo, proporcionando una visión general del proyecto.

### Carpetas

- **`scripts/`**: Código R reutilizable para análisis y visualización.
- **`plots/`**: Gráficos generados durante el análisis, incluyendo PCA y visualizaciones de datos faltantes.
- **`data/`**: Archivos de entrada y resultados procesados (dataset y metadatos).

## Pasos Realizados

1. **Preparación del entorno:** Instalación y carga de las librerías necesarias.
2. **Carga y exploración inicial:** Inspección del dataset para entender su estructura.
3. **Creación del objeto `SummarizedExperiment`:** Organización de los datos en un formato estructurado.
4. **Limpieza y normalización de datos:** Filtrado de metabolitos de baja calidad y transformación logarítmica.
5. **Análisis exploratorio:** Visualización de datos con gráficos de PCA y análisis estadístico univariante.
6. **Resultados y conclusiones:** Interpretación de los resultados obtenidos y sugerencias para próximos pasos.

## Requisitos

Para reproducir este análisis, necesitas los siguientes paquetes de R:

- `SummarizedExperiment`
- `readxl`
- `tidyverse`
- `mixOmics`
- `ggplot2`
- `naniar`
- `impute`

Instálalos ejecutando el siguiente comando en R:

```r
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install(c("SummarizedExperiment", "readxl", "tidyverse", "mixOmics", "ggplot2", "naniar", "impute"))
```

## Cómo Usar Este Repositorio

1. Clona este repositorio:

   ```bash
   git clone https://github.com/AngelPerez/PEC1-Metabolomics.git
   ```

2. Abre el archivo `PEC1.Rmd` o `PEC1.qmd` en RStudio para revisar o ejecutar el análisis.
3. Explora los gráficos y resultados en las carpetas correspondientes.
4. Puedes modificar y ejecutar el código para adaptarlo a otros datasets o propósitos.

## Autor
Ángel Ignacio Pérez Santiago  
Correo: [nuiter@gmail.com](mailto:nuiter@gmail.com)  
