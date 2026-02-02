# 🐍 Script de Análisis: Automatización de Cartera SAP

Esta carpeta contiene el motor lógico del proyecto. El script desarrollado en Python permite transformar datos crudos extraídos de SAP en información estratégica para la toma de decisiones financieras.

## 📋 Funcionalidades del Código
El archivo `sap_aging_analysis.ipynb` ejecuta las siguientes etapas de procesamiento de datos:

* **Simulación de Entorno SAP:** Recreación de estructuras de datos basadas en las tablas **BSID** (Partidas Abiertas) y **BSAD** (Partidas Compensadas).
* **Limpieza y Transformación:** Normalización de montos y cálculo automático de los **Días de Mora** para cada registro.
* **Categorización de Riesgo:** Clasificación de cada partida en "buckets" de antigüedad (Al día, Riesgo Bajo, Riesgo Medio y Crítico +90).
* **Generación de Reporte de Acción:** El script identifica automáticamente a los clientes en estado crítico y genera una alerta con el ID del cliente (Kunnr) y el monto adeudado para intervención inmediata.

## 🛠️ Tecnologías Utilizadas
* **Python 3**
* **Pandas:** Para la manipulación y análisis de estructuras de datos.
* **Matplotlib / Seaborn:** Para la generación de la visualización ejecutiva que se encuentra en la carpeta `visuals`.

---
*Este código está diseñado para ser escalable y puede adaptarse fácilmente a extracciones reales de SAP mediante archivos .csv o conexiones directas.*
