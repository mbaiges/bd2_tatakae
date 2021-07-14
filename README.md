# Trabajo Práctico Base de Datos II - Grupo TATAKAE

## Integrantes

- Baiges, Matías Sebastián  59076
- Bilevich, Andrés Leonardo 59108
- Margossian, Gabriel Viken 59130

## Presentación

[Link a la presentación parcial](https://docs.google.com/presentation/d/13mVJ33jD3wlwoXh5DxbftZTCi2Hl1YvEvEp0AHVJ5oo)

[Link a la presenciación final](https://docs.google.com/presentation/d/1AjDQwQdMtQcjmro00_0LwIOPM7ZLCM4mY7wwDXjoHiA)

## Introducción a RavenDB:

![RavenDB](https://upload.wikimedia.org/wikipedia/commons/9/93/Ravendb-logo.png)

1. Explicación sobre el Alcance y funcionalidades que tiene:
    1. Performance
    2. ACID Transactions
    3. High Availability
    4. Spatial
    5. Full-text search
2. Operaciones CRUD
3. Supported Clients (C#, Java, Node.js, Python, C++, Go)

##Benchmarking


### Comparación <img src="https://user-images.githubusercontent.com/44510239/121270167-9035e480-c897-11eb-9a03-354cd7763f3d.png" width="20" height="20"> con Neo4j 

- Complejidad temporal
  - Búsquedas dentro de una red con más de 1000 nodos
  - Agregado de un nuevo nodo
  - Creación de una coneccion de dos nodos
  - Cuenta de la cantidad de conexiones salientes de un nodo
- Complejidad espacial
  - Espacio que ocupa una red con más de 10000 nodos 
  - Espacio que ocupa una red con 10000 nodos todos conectados entre sí

### Comparación <img src="https://user-images.githubusercontent.com/44510239/121270167-9035e480-c897-11eb-9a03-354cd7763f3d.png" width="20" height="20"> con PostgreSQL

- Complejidad temporal
  - Casos de uso prácticos con transacciones modelo
  - Comparación con Postgis para operaciones geoespaciales

### Comparación <img src="https://user-images.githubusercontent.com/44510239/121270167-9035e480-c897-11eb-9a03-354cd7763f3d.png" width="20" height="20"> con MongoDB

- Complejidad temporal
  - Agregado de documentos json
  - Consulta por clave primaria de json
  - Consulta por elemento según atributo que no pertenezca a clave primaria
- Complejidad espacial
  -Espacio almacenado al agregar 1000 entradas en formato json.

### Comparación <img src="https://user-images.githubusercontent.com/44510239/121270167-9035e480-c897-11eb-9a03-354cd7763f3d.png" width="20" height="20"> con Elastic

- Complejidad temporal
  - Búsquedas por texto contenido en documentos
- Complejidad espacial
  - Creación de una colección con sus índices para hacer búsquedas sobre la misma.
