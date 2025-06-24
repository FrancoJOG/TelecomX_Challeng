
# 📊 Análisis de Pérdida de Clientes (Churn) — Desafío telecomX_latam

## Descripción

Este proyecto corresponde al desafío de análisis de datos propuesto por **Alura/Oracle Next Education** bajo el nombre de **telecomX_latam**.  
El objetivo es analizar los factores que influyen en la pérdida de clientes (Churn) de una empresa de telecomunicaciones, utilizando técnicas de **análisis exploratorio de datos (EDA)** sin aplicar algoritmos de machine learning.

---

## 📦 Dataset

El conjunto de datos contiene 7032 registros de clientes, con información detallada como:

- **Datos demográficos**: Género, edad (SeniorCitizen), dependientes, pareja.
- **Información contractual**: Tipo de contrato, duración, método de pago, facturación electrónica.
- **Servicios contratados**: Tipo de Internet, servicios adicionales como streaming, soporte técnico, etc.
- **Facturación**: Cargos mensuales y totales.
- **Variable objetivo**: `Churn` (Yes/No), indicando si el cliente abandonó el servicio.

---

## ⚙️ Tecnologías y Herramientas

- Python 3.x
- Pandas
- Seaborn
- Matplotlib
- Jupyter Notebook / Google Colab

---

## 📋 Pasos Realizados

1. **Carga y exploración inicial de datos**
   - Revisión de tipos de datos, valores faltantes, descripción estadística básica.
   
2. **Análisis de correlación de variables categóricas con Churn:**
   - Contrato (`Contract`) vs Churn
   - Tipo de servicio de Internet (`InternetService`) vs Churn
   - Método de pago (`PaymentMethod`) vs Churn
   - Edad (`SeniorCitizen`), Pareja (`Partner`), Dependientes (`Dependents`) vs Churn

3. **Cruces múltiples (crosstab) para detección de patrones:**
   - Ejemplo: clientes con contrato "Month-to-month" y pago "Electronic check" presentan mayor tasa de abandono.

4. **Análisis de variables numéricas discretizadas:**
   - Variables como `Charges.Monthly` y `tenure` fueron agrupadas para facilitar su interpretación en relación con Churn.

5. **Identificación de patrones clave y propuesta de acciones de mejora.**

---

## 🔍 Principales Hallazgos

- Los contratos **"Month-to-month"** tienen la tasa más alta de abandono.
- Los pagos realizados por **"Electronic check"** se asocian a mayor churn.
- Clientes con **fibra óptica** presentan mayor probabilidad de abandono en comparación con DSL.
- **Adultos mayores** (SeniorCitizen = 1) abandonan con mayor frecuencia.
- Clientes **sin pareja y sin dependientes** tienden a cancelar el servicio con más frecuencia.
- **Cargos mensuales más altos** están ligeramente relacionados con mayor churn.

---

## 🎯 Propuestas de Mejora

- Ofrecer incentivos y descuentos para contratos de largo plazo (1 o 2 años).
- Promover métodos de pago automáticos mediante beneficios o recompensas.
- Realizar encuestas o mejoras en la oferta de fibra óptica para reducir insatisfacción.
- Diseñar atención personalizada y soporte adaptado para adultos mayores.
- Ajustar planes o precios para reducir la percepción de alto costo mensual.

---

## ▶️ Instrucciones para ejecutar el proyecto

1. Clonar este repositorio:

```bash
git clone https://github.com/tu_usuario/telecomX_latam.git
cd telecomX_latam
```

2. Instalar dependencias:

```bash
pip install pandas seaborn matplotlib
```

3. Ejecutar el notebook `telecomX_latam_analysis.ipynb` en Jupyter o Google Colab.

---

## 📝 Notas

Este proyecto fue desarrollado como parte del programa de formación de datos de **Alura/Oracle Next Education**, con enfoque en análisis exploratorio de datos (EDA) y obtención de insights de negocio sin modelos predictivos.

---

## ✍️ Autor

- Franco Ortega  
- [LinkedIn](linkedin.com/in/franco-joseph-ortega-gutiérrez-368a6a193)  
- [GitHub](https://github.com/FrancoJOG)  
