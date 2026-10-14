# Análisis Exploratorio de Datos: Producción de Carne Bovina en Argentina 🥩🇦🇷

Este repositorio contiene un Análisis Exploratorio de Datos (EDA) exhaustivo sobre el desempeño técnico y económico de la producción de carne bovina en Argentina, considerando diferentes actividades productivas (**Cría**, **Ciclo Completo** e **Invernada**).

---

## 📌 Objetivos del Proyecto

- **Evaluar indicadores económicos**: Analizar la distribución del Margen Bruto ($/ha) y el Resultado Neto ($/ha) entre actividades.
- **Analizar parámetros productivos**: Evaluar el impacto de la Carga Animal (kg/ha), Producción de carne (kg/ha) y Porcentaje de Destete (%).
- **Identificar estructuras de costos**: Comparar la participación de Gastos Directos e Indirectos según el modelo productivo.
- **Relaciones clave**: Estudiar la correlación entre la carga animal y la productividad lograda.

---

## 📊 Principales Hallazgos

1. **Margen Bruto por Actividad**:
   - **Invernada**: Presenta el promedio más alto ($1.296 / ha) y la mayor dispersión/techo productivo.
   - **Ciclo Completo**: Posición intermedia sólida ($1.176 / ha).
   - **Cría**: Margen promedio de $895 / ha, caracterizado por una menor variabilidad.

2. **Resultado Neto ($/ha)**:
   - La mayoría de las unidades productivas se concentran en el rango de **$0 a $500 / ha**, con un promedio general de **$415 / ha**.

3. **Carga Animal vs. Producción**:
   - Existe una **correlación lineal positiva clara** entre la carga animal (kg/ha) y la producción física de carne (kg/ha).
   - La producción en Cría es más limpia y homogénea (30 a 45 kg/ha), mientras que la Invernada alcanza techos cercanos a los 280 kg/ha.

4. **Tratamiento de Datos**:
   - Corrección de valores centinela (`-99999` a `NaN`) en variables como el porcentaje de destete para evitar sesgos en el análisis de Invernada y Ciclo Completo.

---

## 🛠️ Tecnologías Utilizadas

- **Lenguaje**: Python 3.x
- **Librerías principales**:
  - `pandas` & `numpy`: Manipulación y limpieza de datos.
  - `matplotlib` & `seaborn`: Visualización estadística de datos.

---

## 📁 Estructura del Repositorio

```text
.
├── data/
│   └── produccion_carne_argentina.csv   # Dataset base
├── notebooks/
│   └── eda_ganaderia_argentina.ipynb    # Jupyter Notebook con el análisis
└── README.md                            # Descripción del proyecto
