## ANÁLISIS DE FIDELIDAD DE LOS CLIENTES DE UNA AEROLÍNEA
Este proyecto de análisis de datos es un estudio detallado sobre el comportamiento de los clientes de una aerolínea canadiense.

# Descripción del proyecto:
Este trabajo aborda el ciclo completo de un analista de datos: Exploración de datos, limpieza, transformación, análisis de los datos mediante estadística descriptiva e interpretación de resultados.

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
* **Actividad de Vuelo:** Registros de reservas, distancias y puntos acumulados.
* **Historial de Fidelidad:** Perfiles de clientes (salario, educación, ubicación, etc.).

### 2. Limpieza y transformación
Para garantizar la calidad del análisis, se realizaron las siguientes tareas:
* **Unificación de datasets:** Transformación de nombres de columnas a minúsculas y sustitución de espacios por guiones bajos (`_`).
* **Gestión de duplicados:** Eliminación de registros repetidos que podían sesgar los resultados.
* **Filtrado:** Selección de las variables más relevantes para el negocio.

### 3. Tratamiento de Datos Faltantes (Nulos)
Se detectó que un **25.33%** de la columna de salarios no tenía datos. En lugar de descartar esa información, se utilizó **imputación estadística avanzada** para estimar los valores basados en el perfil del cliente, asegurando la integridad del estudio.


# Desarrollo del proyecto:
1. Se crea una función para llamar a la Api donde se contemplan posibles errores a la hora de llamar a la Api.
La Api facilitada es: https://beta.adalab.es/resources/apis/pelis/pelis.json
Se obtienen 100 peliculas con sus datos.
La extracción se realiza con Python utilizando peticiones HTTP y se convierten a formato json.

2. Procesamiento de los datos convirtiendo formato json en un DataFrame desde donde se revisa: posibles valores nulos, tipos de datos y coherencia en los mismos. 
Esto asegura que los datos estén listos para ser insertados en una base de datos.

3. Conexión de Paython a MySQL usando try/expept para contemplar excepciones.
Posteriormente se crea la base de datos bd_peliculas_adalab y la tabla peliculas.

4. Insertar datos

5. Consultas sobre la base de datos creada desde Paython. Para llevarlas a cabo se ha usado los siguientes métodos:
-cursor.execute()
-fetchone() y fetchall() para visualizar los datos de la consulta
- libreria pandas para mostrar los resultados en DataFrame
- el método pd.read_sql_query() para mostrar los resultados directamente desde pandas

6. En la segunda parte se realizan consultas a la base de datos Sakila desde MySQL. Para ello se ha usado el lenguaje SQL.

# Tecnologías utilizadas:
* Paython
* Librerias importadas:
 requests: para conectar con Api y descargar los datos
 pandas as pd: para convertir los datos en formato tabla
 mysql.connector: para conectar Paython con MySQL
 numpy as np: para convertir formato nan de Paython a none de MySQL
 from mysql.connector import Error: captura errores de MySQL
 * MySQL Workbench
 * Git Hub 
 * Visual Studio Code (Jupiter Notebook)

 # Resultado del proyecto:
  Al finalizar este proyecto, se obtiene:
  * Un conjunto de datos limpios con 100 películas.
  * Una base de datos funcional en MySQL.
  * Consultas SQL que permiten analizar la información.