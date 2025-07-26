# Predicción de abandono de clientes - Beta Bank 🏦

Los clientes de **Beta Bank** están abandonando el servicio poco a poco cada mes. Dado que conservar a los clientes actuales resulta más rentable que adquirir nuevos, el objetivo de este proyecto es desarrollar un modelo predictivo que anticipe si un cliente dejará el banco próximamente.

## 🎯 Objetivo

Predecir la probabilidad de que un cliente abandone el banco. Para ello:

- Entrené modelos de clasificación utilizando diversas técnicas de aprendizaje automático.
- Evalué el rendimiento del modelo con la métrica F1 (mínimo requerido: **0.59**).
- Analicé también la métrica **AUC-ROC** para una visión más completa del rendimiento.

## 📂 Dataset

Archivo: `/datasets/Churn.csv`

Contiene los siguientes campos:

- `RowNumber`: índice de fila
- `CustomerId`: ID único del cliente
- `Surname`: apellido
- `CreditScore`: puntuación crediticia
- `Geography`: país de residencia
- `Gender`: sexo
- `Age`: edad
- `Tenure`: años como cliente
- `Balance`: saldo de cuenta
- `NumOfProducts`: productos bancarios contratados
- `HasCrCard`: tiene tarjeta de crédito (1: sí, 0: no)
- `IsActiveMember`: es un miembro activo (1: sí, 0: no)
- `EstimatedSalary`: salario estimado
- `Exited` (target): el cliente se ha ido (1: sí, 0: no)

## 🧠 Técnicas usadas

- Limpieza y preprocesamiento de datos
- Análisis de balance de clases
- Modelado con:
  - Árboles de decisión
  - Bosques aleatorios
  - Regresión logística
- Corrección de desequilibrio con:
  - Submuestreo y sobremuestreo
  - `SMOTE`
  - Ajuste de pesos de clase
- Evaluación con:
  - F1-score
  - Curva ROC y AUC-ROC

## ✅ Resultados

- Mejor modelo alcanzó un **F1-score ≥ 0.59** en el conjunto de prueba.
- Se compararon métricas F1 y AUC-ROC para verificar estabilidad y calidad del modelo.
