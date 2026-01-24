## ANÁLISIS DE FIDELIDAD DE LOS CLIENTES DE UNA AEROLÍNEA
Este proyecto estudia y analiza el comportamiento de los clientes de una aerolínea canadiense entre 2017 y 2018 dentro de un programa de fidelidad.

# Descripción del proyecto:
Este trabajo aborda el ciclo completo de un analista de datos: Exploración de datos, limpieza, transformación, análisis de los datos mediante estadística descriptiva e interpretación de resultados.

# 📂 Estructura del Repositorio
* `notebooks/`: Archivos .ipynb con todo el código documentado.
* `files/`: Carpeta para los datasets originales (CSV).
* `README.md`: Este archivo explicativo.

# Tecnologías utilizadas:
El análisis ha sido desarrollado íntegramente en **Python**, utilizando las siguientes librerías:
* **Pandas y Numpy:** Para la manipulación, limpieza y unión de los datasets.
* **Seaborn y Matplotlib:** Para la creación de visualizaciones y análisis exploratorio gráfico.
* **Scikit-learn:** Para la imputación avanzada de datos faltantes mediante `IterativeImputer`.
* **Git Hub**
* **Visual Studio Code** (Jupiter Notebook)

## 🚀 Fases del Análisis

### 1. Exploración e Identificación
Se crea una función para leer y hacer una exploración inical de los ficheros csv que contienen los datos a analizar.
Se analizaron dos fuentes de datos iniciales:
* **Actividad de Vuelo:** Registros de reservas, distancias y puntos acumulados durante los años 2017 y 2018.
* **Historial de Fidelidad:** Perfiles de clientes (salario, educación, ubicación, etc.).

### 2. Limpieza y transformación
Para garantizar la calidad del análisis, se realizaron las siguientes tareas:
* **Unificación de datasets:** Transformación de nombres de columnas a minúsculas y sustitución de espacios por guiones bajos (`_`).
* **Gestión de duplicados:** Eliminación de registros repetidos que podían sesgar los resultados.
* **Filtrado:** Selección de las variables más relevantes para el negocio.

### 3. Tratamiento de Datos Faltantes (Nulos)
Se detectó que un **25.33%** de la columna de salarios no tenía datos. En lugar de descartar esa información, se utilizó **imputación estadística avanzada** para estimar los valores basados en el perfil del cliente, asegurando la integridad del estudio.

## 4. Cálculo de las principales medidas de estadística descriptiva
* **Medidas de centralización:**Para ver dónde se encuentra el valor promedio o valor típico.
* **Medidas de dispersión:**Para ver la variabilidad de los datos, cómo de agrupado están los datos y cuánto se separan del valor promedio.
* **Medidas de posición relativa:**Para detectar valores extremos(outliers)
* **Medidas de correlación:**Para descubrir cómo se relacionan algunas variables entre sí
* **Visualización** Distintos gráficos que ayudan a entender el comportamiento de las variables.


## 📈 Conclusiones:

## CONCLUSIONES TRAS EL ANÁLISIS:

Tras estudiar 403760 registros de vuelos de 16737 clientes los hallazgos más relevantes que nos cuentan los datos:

* **Crecimiento del número de vuelos** en 2018 con respecto al año anterior, 2017.
* **Ubicación Estratégica:** Existe una altísima concentración de clientes en la provincia de **Ontario (Toronto)**
* **Perfil del cliente:** el 62% de clientes está casado, hay **equidad de género** 50,22% de mujeres y 49,78% de hombres, el 62,55% de los clientes tiene **nivel educativo Bachelor**. En cuanto al nivel salarial de los clientes los datos nos muestran que la mayoría tienen unos ingresos parecidos entorno a 79343 pero hay un grupo reducido de clientes con ingresos mucho más altos o bajos que el resto, lo que hace que el rango salarial entre los clientes sea superior.
* **Tarjeta de fidelidad** más frecuente es la tipo **star** con un 45,55% seguida de **nova** con un 33,90%
* **Actividad:** En promedio los clientes realizan 4 reservas de vuelo al mes pero al estudiar otras medidas muestran que el numero de reservas que más se repite es 0 o 1, estos resultados nos muestra que la mayoría de clientes tiene una actividad baja, mientras que hay un grupo reducido que tienen una actividad mayor, vuelan más por lo que la distancia recorrida es mayor y los puntos acumulados también haciendo que aumente el promedio de reservas, distancia y puntos