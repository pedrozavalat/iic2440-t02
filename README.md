
# Tarea 2 - Procesamiento de Datos Masivos (IIC2440).
Integrantes: Pedro Pablo Zavala Tejos

Primer semestre, 2024. 

## 1. Ejecución 👨🏻‍💻
Para la ejecucion de la tarea se debe realizar en google Collab. Para poder utilizar el algoritmo Map Reduce sobre el grafo de twitter se debe realizar lo siguiente:
1.  Entrar al siguiente link, y poner en el campo de usernames y password los siguientes datos:
    * Username: `twitter`
    * Password: `twitter`
2. Una vez que la base de datos este activa, solo se requiere ejecutar el codigo de la tarea. Tener en cuenta que siempre la autentificacion para acceder a la base de datos en neo4j desde el colab es la misma: 
```python
    NEO4J_URI = "neo4j+s://demo.neo4jlabs.com"
    NEO4J_USERNAME = "twitter"
    NEO4J_PASSWORD = "twitter"
    AUTH = (NEO4J_USERNAME, NEO4J_PASSWORD)
```
3. Una vez ejecutado, se podran ver los resultados (no se requiere descargar nada, solo trabajamos desde la nube).

## 2. Links importantes 🔗
* Demo Twitter Database Neo4j: [Link](https://demo.neo4jlabs.com:7473/browser/?dbms=neo4j://twitter@demo.neo4jlabs.com&db=twitter)
* Video de Youtube
## 3. Carpetas y Archivos 📂
* `imgs`: Carpeta con las imagenes de los grafos resultantes para las 2 consultas realizadas que se muestran en el video.
* `neo4j-queries`: Carpeta con las consultas realizadas en Neo4j que permiten entregar los grafos mostrados en el video de youtube. 
* `graphsMapReduce.ipynb`: Colab con el codigo de la tarea. 

