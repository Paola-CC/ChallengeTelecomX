# 📊 Telecom X: Análisis de Retención de Clientes (Churn)
### Proyecto de Ciencia de Datos Junior | Análisis Estratégico de Negocio

Este repositorio contiene el análisis técnico y estratégico realizado para **Telecom X**, una empresa de telecomunicaciones que enfrenta una tasa de cancelación del **25.7%**. El objetivo es identificar patrones de comportamiento y proponer soluciones para mejorar la lealtad del cliente.

---

## 📋 Resumen del Proyecto
La pérdida de clientes (Churn) es uno de los mayores desafíos en la industria de telecomunicaciones. Este proyecto utiliza Python para transformar datos crudos en información accionable, siguiendo el ciclo de vida de un proyecto de datos: **ETL** y **EDA**.



## 🛠️ Tecnologías y Librerías
* **Lenguaje:** Python 3.x
* **Manipulación de Datos:** `Pandas`, `NumPy`
* **Visualización:** `Matplotlib`, `Seaborn`
* **Extracción:** `Requests` (Consumo de API JSON)

---

## ⚙️ Metodología Aplicada

### 1. Extracción (ETL)
Se importaron los datos desde una API externa con una estructura JSON anidada.
* **Acción:** Se normalizaron las categorías `customer`, `phone`, `internet` y `account` para crear un dataset único y plano (`df_final`).

### 2. Transformación y Limpieza
Para asegurar la calidad del análisis, se realizaron las siguientes tareas:
* **Limpieza de Errores:** Conversión de `Charges.Total` a valores numéricos, gestionando espacios en blanco y valores nulos.
* **Automatización:** Creación de funciones de conversión binaria (0 y 1) para variables como Género, Churn, y servicios adicionales.
* **Ingeniería de Características:** Creación de la columna `Cuentas_Diarias` para analizar el gasto prorrateado por día.

### 3. Análisis Exploratorio de Datos (EDA)
Se realizaron cruces de variables para entender el "porqué" de las cancelaciones:
* **Análisis de Tenencia:** Identificación de la ventana de riesgo (meses 1 a 10).
* **Análisis de Servicios:** Evaluación del impacto de la Fibra Óptica y los servicios de Seguridad Online.
* **Comportamiento Financiero:** Relación entre el método de pago y la permanencia.

---

## 📂 Estructura del Repositorio
* `TelecomX_Analysis.ipynb`: Notebook principal con el código de limpieza y visualización.
* `TelecomX_Data.json`: Fuente de datos original (vía URL).
* `README.md`: Resumen ejecutivo y técnico del proyecto.
