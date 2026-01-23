## Análisis de Fidelidad y Actividad de Vuelo de Clientes ✈️

 Este proyecto de análisis de datos es un estudio detallado sobre el comportamiento de los clientes de una aerolínea canadiense. El objetivo principal fue unificar datos de vuelos con perfiles demográficos para extraer información valiosa sobre la fidelidad y el uso del servicio.

## 📊 Resumen del Proyecto

Este trabajo aborda el ciclo completo de un analista de datos: Exploración de datos, limpieza, transformación, análisis de los datos mediante estadística descriptiva e interpretación de resultados.

## 🛠️ Herramientas utilizadas

El análisis ha sido desarrollado íntegramente en **Python**, utilizando las siguientes librerías:
* **Pandas y Numpy:** Para la manipulación, limpieza y unión de los datasets.
* **Seaborn y Matplotlib:** Para la creación de visualizaciones y análisis exploratorio gráfico.
* **Scikit-learn:** Para la imputación avanzada de datos faltantes mediante `IterativeImputer`.

## 🚀 Fases del Análisis

### 1. Exploración e Identificación
Se analizaron dos fuentes de datos iniciales:
* **Actividad de Vuelo:** Registros de reservas, distancias y puntos acumulados.
* **Historial de Fidelidad:** Perfiles de clientes (salario, educación, ubicación, etc.).

### 2. Limpieza y transformación
Para garantizar la calidad del análisis, se realizaron las siguientes tareas:
* **Unificación de datasets:** Transformación de nombres de columnas a minúsculas y sustitución de espacios por guiones bajos (`_`).
* **Gestión de duplicados:** Eliminación de registros repetidos que podían sesgar los resultados.
* **Filtrado:** Selección de las variables más relevantes para el negocio.

### 3. Tratamiento de Datos Faltantes (Nulos)
Se detectó que un **25.33%** de la columna de salarios no tenía datos. En lugar de descartar esa información, se utilizó **imputación estadística avanzada** para estimar los valores basados en el perfil del cliente, asegurando la integridad del estudio.

---

## 📈 Conclusiones Clave (Insights de Datos)

Tras analizar los datos finales, estos son los hallazgos más relevantes:

* **Perfil del Cliente:** El cliente promedio tiene un nivel educativo de **Grado (Bachelor)** y el grupo demográfico más grande está compuesto por personas **casadas**.
* **Actividad:** En promedio, los clientes realizan **4 reservas por periodo**, aunque existe un segmento de alta frecuencia que llega hasta las 21 reservas.
* **Poder Adquisitivo:** El salario promedio estimado de la base de clientes se sitúa en **79,343 unidades**.
* **Ubicación Estratégica:** Existe una altísima concentración de clientes en la provincia de **Ontario (Toronto)**, lo que sugiere que es el núcleo principal de la operación.
* **Equidad de Género:** El programa de fidelidad es muy equilibrado, con una presencia ligeramente superior de **mujeres (8,410)** frente a hombres.

---

## 📂 Estructura del Repositorio
* `notebooks/`: Archivos .ipynb con todo el código documentado.
* `files/`: Carpeta para los datasets originales (CSV).
* `README.md`: Este archivo explicativo.


