# Proyecto de Machine Learning: Detección de Fibrilación Auricular (AFib)

Este repositorio contiene el proyecto del curso de Machine Learning, donde se entrena y evalúa un clasificador supervisado para distinguir entre señales ECG normales y con fibrilación auricular.

## Objetivo

Entrenar un modelo de clasificación utilizando Random Forest y evaluar su desempeño con métricas estándar (Accuracy, Precision, Recall, F1-score) y visualización de la matriz de confusión.

## Estructura del repositorio

```
Datos De Prueba/
├── ecg_rr_features_curado.csv     # CSV con características HRV extraídas (30 registros)
├── Semana2_ReproduccionBaseline.ipynb  # Entrenamiento y evaluación del modelo
├── Semana_1_Exploracion.ipynb          # Análisis exploratorio y extracción de features
└── README-Leer antes de ejecutar ...   # Este archivo
```

## Descripción de los datos

* Se trabajó con 30 registros de ECG (15 normales, 15 AFib) procesados para extraer características de variabilidad de frecuencia cardíaca (HRV).
* Para cada registro se calculan estadísticas de intervalos RR: promedio, desviación estándar, RMSSD, pNN50, asimetría y curtosis.
* El archivo `ecg_rr_features_curado.csv` contiene estas características más la etiqueta `label` (0=Normal, 1=AFib).

## Notebooks

1. **Semana 1: Exploración del dataset**  
   Ruta: `Semana_1_Exploracion.ipynb`
   * Carga y procesamiento de señales ECG
   * Detección de picos R y cálculo de intervalos RR
   * Extracción de características HRV y guardado en CSV
   * Análisis de distribuciones y visualizaciones exploratorias

2. **Semana 2: Reproducción del baseline**  
   Ruta: `Semana2_ReproduccionBaseline.ipynb`
   * División de datos en train/test con `train_test_split`
   * Entrenamiento de un clasificador Random Forest
   * Cálculo de Accuracy, Precision, Recall, F1-score
   * Visualización de la matriz de confusión e importancia de características
   * Análisis de resultados y conclusiones

## Instrucciones para ejecutar

1. Clonar o descargar el repositorio
2. Instalar dependencias (idealmente en un entorno virtual):
3. Y con esos pasos debería de ser capaz de ejecutar el proyecto

=======================================================================================================================
Semana 1:

Saludos profesor, para el proyecto que ML todo lo he realizado en (jupyter notebook), así que no debería tener problemas para ejecutarlo, mi primera entrega se compone de 2 partes.

1)La primera en donde se realizan las pruebas con los datos (csv) que usted dejó en educandus.

2)Y la segunda ya son con datos reales extraídos de training2017, el archivo original se compone con más de 17000 casos de prueba de los cuales solamente realicé pruebas con solo 500, puesto que para probar solo era necesario utilizar 30, pero en el propio código puede revisar esa variable y modificarla según estime conveniente.

=======================================================================================================================

Semana 2:

Saludos profesor, solo como información no podré entregar el git como lo solicitó (con el orden de las carpetas), puesto que como estoy usando el mismo repositorio de git, debería de modificar la entrega 1, lo cual diría que no está permitido.