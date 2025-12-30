# Telecom-X
Análisis de Evasión de Clientes (Churn)

Este proyecto forma parte de un desafío de Data Science enfocado en el sector de telecomunicaciones. El objetivo principal es analizar el comportamiento de los clientes para identificar los factores que influyen en la cancelación de servicios (Churn) y proponer estrategias basadas en datos para mejorar la retención.

## 📁 Estructura del Proyecto

* `TelecomX_Data.json`: Dataset original con información de clientes, servicios y facturación.
* `TelecomX_LATAM.ipynb`: Notebook de Python con el proceso de extracción, transformación y análisis.
* `TelecomX_diccionario.md`: Diccionario de datos detallando cada variable.
* !(img/Churn.png)
* !(img/Cantidad de Clientes por Churn.png)

## 🛠️ Tecnologías Utilizadas

* **Python 3.x**
* **Pandas**: Manipulación y normalización de datos JSON.
* **Matplotlib**: Visualización de datos y análisis gráfico.
* **JSON**: Manejo de estructuras de datos anidadas.

## 🚀 Proceso de Datos (ETL)

1. **Extracción:** Carga de datos desde archivos JSON complejos con múltiples niveles de anidación.
2. **Transformación:** - Normalización de columnas anidadas (`customer`, `phone`, `internet`, `account`).
   - Limpieza de datos: Identificación y tratamiento de 11 valores nulos en la facturación total (clientes con antigüedad 0).
   - Ingeniería de variables: Creación de la métrica `Cuentas_Diarias` para un análisis más granular.
3. **Análisis:** Evaluación descriptiva y visualización de variables clave.



## 📈 Hallazgos Principales

* **Tasa de Churn:** El **26.5%** de la base de clientes ha abandonado el servicio.
* **Periodo de Riesgo:** La mayor probabilidad de abandono ocurre en los primeros **12 meses** de antigüedad.
* **Tipo de Contrato:** Los contratos "Mes a mes" son los más volátiles, mientras que los contratos a largo plazo aseguran la permanencia.
* **Impacto Financiero:** Los clientes que cancelan suelen tener cargos mensuales más elevados que el promedio de clientes leales.

## 💡 Recomendaciones Estratégicas

* Implementar planes de fidelización enfocados en los primeros 6 meses de vida del cliente.
* Crear incentivos para migrar a clientes de contratos mensuales a contratos anuales.
* Monitorear a los clientes con cargos mensuales altos para ofrecerles planes ajustados antes de que decidan cancelar.

---
Producido por Cristian Galati - 2025
