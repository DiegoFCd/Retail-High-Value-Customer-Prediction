# Retail High-Value Customer Prediction 
<br>

## 🚀 Project Overview

Este proyecto aplica técnicas de Machine Learning para identificar clientes con alta probabilidad de generar valor comercial futuro.

Representa la evolución predictiva de mi proyecto anterior de Business Intelligence:

---
## 📊 Retail Sales Analysis Supermercados Pronta <br>
👉 (https://github.com/DiegoFCd/Pronta_Supermercados) 

Mientras que el proyecto original de BI se centraba en comprender los patrones históricos de ventas y el comportamiento del cliente, 
este proyecto se centra en predecir qué clientes tienen más probabilidades de convertirse en Clientes de Alto Valor en el futuro.

---
<br>

## 🎯 Business Objective

Las empresas suelen invertir recursos de marketing y retención en toda su base de clientes sin distinguir a aquellos con mayor potencial de ingresos futuros.

El objetivo de este proyecto es identificar a los Clientes de Alto Valor con anticipación, lo que permite una asignación más eficiente de los esfuerzos de marketing, los programas de fidelización y las estrategias de retención.

---
<br>

## 📈 Project Objectives
- Analizar el comportamiento de compra del cliente
- Desarrollar funcionalidades orientadas al negocio
- Estimar el valor futuro del cliente
- Identificar clientes de alto valor
- Entrenar y evaluar un modelo de aprendizaje automático
- Traducir los resultados del modelo en información útil para el negocio

---
<br>


## 📷 Analytics evolution diagram
```text
Retail Sales Analysis (BI)
↓
Customer Behavior Analysis
↓
Feature Engineering
↓
Future CLV Estimation
↓
High Value Customer Prediction
```
---
<br>

## 💡 Dataset

**El proyecto utiliza datos transaccionales de venta minorista a nivel de cliente.**

El conjunto de datos original contiene:

- ID del cliente
- Información de la factura
- Compras de productos
- Fechas de transacción
- Cantidad comprada
- Ingresos generados

**Durante la fase de Features Engineering, el conjunto de datos se transformó en un conjunto de datos analíticos centrado en el cliente, que incluye:**

- Recencia
- Frecuencia
- Valor monetario
- Tiempo promedio de compra
- Intervalo promedio de compra
- Valor de vida del cliente futuro (CLV futuro)

**Estas características se utilizaron posteriormente para entrenar el modelo de Machine Learning responsable de identificar a los clientes de alto valor.**

---
<br>

## 📷 Project Workflow

**🔧 Features Engineering**

Se crearon variables de comportamiento del cliente a partir del historial de transacciones.

**Principales características:**

- Average Ticket
- Monetary Value
- Recency
- Average Purchase Interval

Estas variables resumen el comportamiento de compra y proporcionan información relevante para la predicción del valor del cliente.

---
<br>

## 🎯 Target Construction

El valor de vida del cliente futuro (CLV futuro) se calculó utilizando transacciones futuras.

Los clientes se clasificaron en:

- 1 = Cliente de alto valor
- 0 = Cliente habitual

Esta transformación permitió abordar el problema como una tarea de clasificación binaria.

--- 
<br>

## 🧠Model Used

**Random Forest Classifier**

El modelo se entrenó para identificar a los clientes con mayor probabilidad de convertirse en clientes de alto valor.

¿Por qué RandomForest?

- Maneja relaciones no lineales
- Funciona bien con características diseñadas
- Proporciona interpretación de la importancia de las características
- Robusto ante comportamientos de venta volátiles

---
<br>

## 📊 Model Performance

### Métricas de rendimiento

| Metric | Score |
|----------|----------|
| Precision (High Value) | 20% |
|Recall (High Value) | 78% |
| F1-Score | 32% |
|Threshold Optimization | 0.40 |

El umbral de clasificación se ajustó para priorizar la detección de clientes de alto valor.

Esto aumentó la exhaustividad a aproximadamente un 78%, lo que permitió al modelo identificar a la mayoría de los futuros clientes de alto valor, aunque aceptando un mayor número de falsos positivos.

---
<br>

## 📷 Confusion Matrix

![Analytics Evolution](outputs/confusion-matrix.png)

<br>

### 📊 Confusion Matrix Interpretation

Tras la optimización del umbral, el modelo identificó correctamente aproximadamente el **78 % de los futuros clientes de alto valor**.

El umbral se ajustó para priorizar la detección de clientes (Recall), asegurando así la captación de la mayoría de los clientes con alto potencial, incluso a costa de generar falsos positivos adicionales.

---
<br>

## 🔍 Feature Importance

Las variables más influyentes para predecir el valor futuro del cliente fueron:

- Average Ticket
- Monetary Value
- Recency
- Average Purchase Interval

**Estas características proporcionan información valiosa sobre los patrones de comportamiento asociados a los clientes de alto valor.** 

---
<br>

## 💼 Business Value

Este modelo puede ayudar a las organizaciones a:

- Priorizar a los clientes con alto potencial
- Mejorar la segmentación de marketing
- Optimizar las campañas de fidelización
- Aumentar el valor de vida del cliente
- Apoyar la toma de decisiones basada en datos

---
<br>

## 🛠 Technologies Used
- Python
- Pandas
- NumPy
- Scikit-Learn
- Random Forest
- Matplotlib
- Seaborn
- Google Colab

---
<br>

## 🔗 Related Project

 📊 Retail Sales Analysis Supermercados Pronta 👉 (https://github.com/DiegoFCd/Pronta_Supermercados)

Este proyecto amplía el análisis original de Business Intelligence, pasando de:

"¿Qué sucedió?" a ¿Qué es probable que suceda a continuación?"

Mediante análisis predictivo y aprendizaje automático.
