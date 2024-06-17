
# Tarea 2 - Procesamiento de Datos Masivos (IIC2440).
Integrantes: Pedro Pablo Zavala Tejos

Primer semestre, 2024. 

## 0. Importante 🚨❗️
Despues de grabar el video que se encuentra en youtube me di cuenta que me falto considerar la lista de variables que se tenian que recibir en el bullet 4 del enunciado (es decir, A, L y luego generar una matriz M de AxLxA). En consecuencia, para toda consulta en donde debiamos encontrar subgrafos de solamente 4 variables realice lo siguiente

* Antes usabamos la funcion `bgp_query` que retornaba los matches mediante una iteracion lineal (esto fue lo que se mostró en el video). 

* Ahora cree una nueva funcion que reemplaza la funcionalidad de `bgp_query`. Esta funcion se llama `get_matches`, cuyos parametros son iguales que `bgp_query`. Esta retorna todos los matches posibles segun el patron de grafo de la consulta. La idea de esta funcion es crear una matriz de tamaño AxLxA tal que cada celda de la matriz de 3 dimensiones presenta un 1 si existe la arista entre los nodos correspondientes y un 0 en caso contrario. En consecuencia, al procesar una matriz para cada subgrafo encontrado con MapReduce, verificamos que su matriz M sea igual a la matriz de la consulta.

* `get_matches` solo la utiliza en las subsecciones **"MapReduce Algorithm for Squares"**. 


## 1. Ejecución 👨🏻‍💻
Para la ejecucion de la tarea se debe realizar en google Collab. Para poder utilizar el algoritmo Map Reduce sobre el grafo de twitter se debe realizar lo siguiente:
1.  Entrar al siguiente link [Twitter](https://demo.neo4jlabs.com:7473/browser/?dbms=neo4j://twitter@demo.neo4jlabs.com&db=twitter), y poner en el campo de usernames y password los siguientes datos:
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
* Video de Youtube: [IIC2440 Tarea 2 - Map Reduce](https://youtu.be/TZD3ITaT__U)
## 3. Carpetas y Archivos 📂
* `imgs`: Carpeta con las imagenes de los grafos resultantes para las 2 consultas realizadas que se muestran en el video.
* `neo4j-queries`: Carpeta con las consultas realizadas en Neo4j que permiten entregar los grafos mostrados en el video de youtube. 
* `graphsMapReduce.ipynb`: Colab con el codigo de la tarea. 

