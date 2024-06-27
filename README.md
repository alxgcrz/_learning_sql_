# Lenguaje SQL

... EN DESARROLLO ...

## Introducción

**SQL**, que significa **_"Structured Query Language"_** (Lenguaje de Consulta Estructurado), es un lenguaje de programación utilizado para gestionar y manipular bases de datos relacionales. Fue desarrollado en la década de 1970 en IBM basándose en el trabajo de Edgard Codd y se ha convertido en el estándar de facto para interactuar con sistemas de gestión de bases de datos relacionales (SGBDR).

La primera versión de SQL normalizada por ANSI data de 1986. La norma SQL2 o SQL92 es la más importante y la mayoría de los SGBDR existentes implementan esta
versión.

Características clave de SQL:

- **Declarativo**: SQL es un lenguaje de programación declarativo, lo que significa que describe el resultado deseado sin especificar el método para alcanzarlo. Esto permite a los usuarios centrarse en lo que quieren obtener, en lugar de cómo lograrlo.

- **Gestión de datos relacional**: SQL se utiliza principalmente en entornos de bases de datos relacionales, donde la información se organiza en tablas con relaciones entre ellas. Esto facilita la gestión y recuperación eficiente de datos.

- **Manipulación de datos**: SQL permite realizar operaciones fundamentales sobre datos, como la inserción (INSERT), la actualización (UPDATE), la eliminación (DELETE), y la recuperación (SELECT) de información de la base de datos.

- **Creación y modificación de estructuras de datos**: SQL también se utiliza para definir y modificar la estructura de las bases de datos, mediante la creación de tablas (CREATE TABLE), la alteración de tablas (ALTER TABLE), y la eliminación de tablas (DROP TABLE).

- **Consulta de datos**: La sentencia SELECT es esencial en SQL y se utiliza para recuperar datos de una o varias tablas. Permite filtrar, ordenar y agrupar información según las necesidades del usuario.

- **Integridad de datos**: SQL garantiza la integridad de los datos mediante restricciones como claves primarias, claves foráneas y otros mecanismos que aseguran la consistencia y fiabilidad de la información almacenada.

- **Transacciones**: SQL ofrece soporte para transacciones, permitiendo agrupar varias operaciones en una unidad atómica. Esto asegura que todas las operaciones se realicen con éxito o ninguna de ellas.

SQL se ha convertido en una herramienta esencial para cualquier persona involucrada en el desarrollo de software, administración de bases de datos, análisis de datos y otras disciplinas relacionadas con el manejo de información estructurada. Con su amplia adopción, el conocimiento de SQL es valioso en diversos contextos profesionales.

> Sección generada por ChatGPT

El lenguaje SQL se divide en varios subconjuntos:

- **DDL** (_Data Definition Language_), que agrupa todos los comandos utilizados para crear, modificar o eliminar las estructuras de la base de datos (tablas, índices, vistas, etc.). Se trata principalmente de los comandos CREATE, ALTER y DROP.

- **DML** (_Data Manipulation Language_), que agrupa los comandos utilizados para manipular los datos contenidos en la base de datos. Se trata principalmente de los comandos SELECT, INSERT, DELETE y UPDATE.

- **DCL** (_Data Control Language_), que agrupa los comandos utilizados para administrar la seguridad de acceso a los datos. Se trata principalmente de los comandos GRANT y REVOKE.

- **TCL** (_Transaction Control Language_), que agrupa los comandos utilizados para administrar la confirmación o no de actualizaciones realizadas sobre la base de datos. Se trata principalmente de los comandos COMMIT y ROLLBACK

## Introducción a las Bases de Datos Relacionales

El modelo relacional fue creado por un investigador, Edgard Codd, que trabajaba en IBM a principios de los años 70.

El modelo relacional se basa en el concepto de conjunto. Esquemáticamente el modelo relacional se puede representar a través de una tabla; igualmente se puede llamar una tabla, una relación.

Este conjunto tiene atributos (las columnas) y líneas que contienen los valores (los registros).

El modelo relacional presenta los datos de forma lógica, es totalmente independiente del modelo físico. Es el proveedor el que decide el modo de almacenamiento físico de las tablas. Esta es la mayor ventaja de las bases de datos relacionales, la independencia entre lo lógico y lo físico.

Una vez se han definido las tablas, hay que disponer de un lenguaje para manipularlas, se trata del álgebra relacional.

SQL implementa el álgebra relacional y los sistemas de gestión de bases de datos relacionales (SGBDR) implementan el modelo relacional.

Los tres principales conceptos del modelo relacional son el **dominio**, el **producto cartesiano** y las **relaciones**.

### Dominio

El dominio es un conjunto de valores representado por un nombre.

El número de ocurrencias de cada uno de los dominios da la **cardinalidad**.

### Definición de bases de datos y tablas

... PENDIENTE ...

### Tipos de datos

... PENDIENTE ...

## Operaciones básicas con datos

### `SELECT`: Recuperación de datos

... PENDIENTE ...

### `INSERT`: Inserción de nuevos registros

... PENDIENTE ...

### `UPDATE`: Modificación de registros existentes

... PENDIENTE ...

### `DELETE`: Eliminación de registros

... PENDIENTE ...

## Claúsulas y operadores

### `WHERE`: Filtrado de resultados

... PENDIENTE ...

### `ORDER BY`: Ordenamiento de resultados

... PENDIENTE ...

### `GROUP BY`: Agrupación de datos

... PENDIENTE ...

### `HAVING`: Filtrado de resultados agrupados

... PENDIENTE ...

## Joins y relaciones

### Tipos de Joins (INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN)

... PENDIENTE ...

### Claves primarias y foráneas

... PENDIENTE ...

### Relaciones uno a uno, uno a muchos y muchos a muchos

... PENDIENTE ...

## Creación y modificación de tablas

### `CREATE TABLE`: Creación de tablas

... PENDIENTE ...

### `ALTER TABLE`: Modificación de estructuras de tablas

... PENDIENTE ...

### `DROP TABLE`: Eliminación de tablas

... PENDIENTE ...

## Restricciones y índices

### Claves primarias y foráneas

... PENDIENTE ...

### Restricciones de unicidad y nulidad

... PENDIENTE ...

### Creación de índices

... PENDIENTE ...

## Funciones de agregación

### `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`

... PENDIENTE ...

### Uso de funciones en consultas

... PENDIENTE ...

## Subconsultas y Expresiones Comunes de Tabla (CTE)

### Subconsultas anidadas

... PENDIENTE ...

### Uso de CTE para simplificar consultas

... PENDIENTE ...

## Procedimientos almacenados y disparadores ('Triggers')

### Creación y ejecución de procedimientos almacenados

... PENDIENTE ...

### Activación de disparadores en eventos específicos

... PENDIENTE ...

## Gestión de transacciones

### `COMMIT` y `ROLLBACK`

... PENDIENTE ...

### Control de transacciones

... PENDIENTE ...

## Seguridad y privilegios

### Concesión y revocación de privilegios

... PENDIENTE ...

### Control de acceso a datos

... PENDIENTE ...

## Optimización de consultas

### Uso eficiente de índices

... PENDIENTE ...

### Análisis de planes de ejecución

... PENDIENTE ...

---

## Enlaces de interés

- <https://roadmap.sh/sql>
- <https://www.sqltutorial.org/>
- <https://www.sqlitetutorial.net/>
- <https://datalemur.com/sql-tutorial>
- <https://github.com/XD-DENG/SQL-exercise>
- <https://www.w3schools.com/sql/default.asp>
- <https://www.sqlzoo.net/wiki/SQL_Tutorial>
- <https://sqlbolt.com/>
- <https://bookdown.org/paranedagarcia/database/sql.html>

## Licencia

[![Licencia de Creative Commons](https://i.creativecommons.org/l/by-sa/4.0/80x15.png)](http://creativecommons.org/licenses/by-sa/4.0/)
Esta obra está bajo una [licencia de Creative Commons Reconocimiento-Compartir Igual 4.0 Internacional](http://creativecommons.org/licenses/by-sa/4.0/).
