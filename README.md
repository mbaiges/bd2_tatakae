# Trabajo Práctico Base de Datos II - Grupo TATAKAE

## Integrantes

- Baiges, Matías Sebastián
- Bilevich, Andrés Leonardo
- Margossian, Gabriel Viken 

## Presentación

[Link a la presentación](https://docs.google.com/presentation/d/13mVJ33jD3wlwoXh5DxbftZTCi2Hl1YvEvEp0AHVJ5oo)

## Introducción a RavenDB:

1. Explicación sobre el Alcance y funcionalidades que tiene:
  1. Performance
  2. ACID Transactions
  3. High Availability
  4. Full-text search
2. Operaciones CRUD
3. Supported Clients (C#, Java, Node.js, Python, C++, Go)

##Benchmarking

### Comparación con Neo4j

- Complejidad temporal
  - Búsquedas dentro de una red con más de 1000 nodos
  - Agregado de un nuevo nodo
  - Creación de una coneccion de dos nodos
  - Cuenta de la cantidad de conexiones salientes de un nodo
- Complejidad espacial
  - Espacio que ocupa una red con más de 10000 nodos 
  - Espacio que ocupa una red con 10000 nodos todos conectados entre sí

### Comparación con PostgreSQL

- Complejidad temporal
  - Casos de uso prácticos con transacciones modelo
  - Comparación con Postgis para operaciones geoespaciales

### Comparación con MongoDB

- Complejidad temporal
  - Agregado de documentos json
  - Consulta por clave primaria de json
  - Consulta por elemento según atributo que no pertenezca a clave primaria
- Complejidad espacial
  -Espacio almacenado al agregar 1000 entradas en formato json.

### Comparación con Elastic

- Complejidad temporal
  - Búsquedas por texto contenido en documentos
- Complejidad espacial
  - Creación de una colección con sus índices para hacer búsquedas sobre la misma.
