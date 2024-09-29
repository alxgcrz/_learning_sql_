# Lenguaje SQL

> :warning: **EN DESARROLLO** :warning:

## Introducción

**SQL**, que significa **_"Structured Query Language"_** (Lenguaje de Consulta Estructurado), es un lenguaje de programación utilizado para gestionar y manipular bases de datos relacionales. Fue desarrollado en la década de 1970 en IBM basándose en el trabajo de Edgard Codd y se ha convertido en el estándar de facto para interactuar con sistemas de gestión de bases de datos relacionales (SGBDR).

La primera versión de SQL normalizada por ANSI data de 1986. La norma SQL2 o SQL92 es la más importante y la mayoría de los SGBDR existentes implementan esta versión.

Características clave de SQL:

- **Declarativo**: SQL es un lenguaje de programación declarativo, lo que significa que describe el resultado deseado sin especificar el método para alcanzarlo. Esto permite a los usuarios centrarse en lo que quieren obtener, en lugar de cómo lograrlo.

- **Gestión de datos relacional**: SQL se utiliza principalmente en entornos de bases de datos relacionales, donde la información se organiza en tablas con relaciones entre ellas. Esto facilita la gestión y recuperación eficiente de datos.

- **Manipulación de datos**: SQL permite realizar operaciones fundamentales sobre datos, como la inserción (INSERT), la actualización (UPDATE), la eliminación (DELETE), y la recuperación (SELECT) de información de la base de datos.

- **Creación y modificación de estructuras de datos**: SQL también se utiliza para definir y modificar la estructura de las bases de datos, mediante la creación de tablas (CREATE TABLE), la alteración de tablas (ALTER TABLE), y la eliminación de tablas (DROP TABLE).

- **Consulta de datos**: La sentencia SELECT es esencial en SQL y se utiliza para recuperar datos de una o varias tablas. Permite filtrar, ordenar y agrupar información según las necesidades del usuario.

- **Integridad de datos**: SQL garantiza la integridad de los datos mediante restricciones como claves primarias, claves foráneas y otros mecanismos que aseguran la consistencia y fiabilidad de la información almacenada.

- **Transacciones**: SQL ofrece soporte para transacciones, permitiendo agrupar varias operaciones en una unidad atómica. Esto asegura que todas las operaciones se realicen con éxito o ninguna de ellas.

SQL se ha convertido en una herramienta esencial para cualquier persona involucrada en el desarrollo de software, administración de bases de datos, análisis de datos y otras disciplinas relacionadas con el manejo de información estructurada. Con su amplia adopción, el conocimiento de SQL es valioso en diversos contextos profesionales.

> :warning: **Sección introductoria generada por ChatGPT**

El lenguaje SQL se divide en cuatro subconjuntos:

- **DDL** (_Data Definition Language_), que agrupa todos los comandos utilizados para crear, modificar o eliminar las estructuras de la base de datos (tablas, índices, vistas, etc.). Se trata principalmente de los comandos CREATE, ALTER y DROP.

- **DML** (_Data Manipulation Language_), que agrupa los comandos utilizados para manipular los datos contenidos en la base de datos. Se trata principalmente de los comandos SELECT, INSERT, DELETE y UPDATE.

- **DCL** (_Data Control Language_), que agrupa los comandos utilizados para administrar la seguridad de acceso a los datos. Se trata principalmente de los comandos GRANT y REVOKE.

- **TCL** (_Transaction Control Language_), que agrupa los comandos utilizados para administrar la confirmación o no de actualizaciones realizadas sobre la base de datos. Se trata principalmente de los comandos COMMIT y ROLLBACK

## Introducción a las Bases de Datos Relacionales

El modelo relacional fue creado por **Edgar Codd**, un investigador que trabajaba en IBM a principios de los años 70. Su trabajo pionero, "_A Relational Model of Data for Large Shared Data Banks_", sentó las bases de este modelo.

El modelo relacional se basa en el concepto de **conjunto**. Esquemáticamente, el modelo relacional se puede representar a través de una **tabla**, que en términos relacionales es una representación de una relación. Cada fila en la tabla corresponde a una **tupla (o registro)**, y cada columna representa un **atributo**.

> En el modelo relacional, el término **relación** se utiliza para referirse a una tabla, mientras que el término **tupla** se utiliza para referise a una fila. De forma similar, el término **atributo** se refiere a una columna de la tabla.

Este modelo presenta los datos de forma lógica, independientemente del modelo físico. El proveedor de la base de datos decide el modo de almacenamiento físico de las tablas. Esta independencia entre lo lógico y lo físico es una de las mayores ventajas de las bases de datos relacionales.

Una vez definidas las tablas, es necesario un lenguaje para manipularlas, lo cual se logra a través del **álgebra relacional**. Este formalismo matemático permite realizar operaciones sobre conjuntos de datos, como selecciones, proyecciones y uniones.

**SQL** implementa el álgebra relacional, y los sistemas de gestión de bases de datos relacionales (SGBDR) son los encargados de implementar el modelo relacional en la práctica.

Los tres principales conceptos del modelo relacional son el **dominio**, el **producto cartesiano** y las **relaciones**.

### Dominio

El dominio es el **conjunto de posibles valores** que un atributo puede tomar, representado por un nombre. Por ejemplo, el atributo `edad` en una tabla de personas puede tener como dominio el conjunto de números enteros positivos (edad ≥ 0). Si otro atributo es `nombre`, el dominio puede ser el conjunto de todas las cadenas de texto válidas.

Si tenemos un atributo `estado civil`, su dominio podría ser {"soltero", "casado", "divorciado", "viudo"}.

El número de elementos en un dominio se denomina **cardinalidad**. En el ejemplo anterior, la cardinalidad del dominio `estado civil` es 4.

## Álgebra relacional

### Producto cartesiano

El **producto cartesiano** P entre varios dominios D1, D2, ..., Dn, se expresa como P = D1 x D2 x ... x Dn. Este producto representa todas las **combinaciones posibles** de los valores en esos dominios.

Si tenemos dos dominios D1={1,2} y D2={"A", "B"}, el producto cartesiano de D1 y D2 sería:

- P = {(1, "A"), (1, "B"), (2, "A"), (2, "B")}

Cada par de valores es una tupla (d1, d2), donde "d1" proviene de D1 y "d2" proviene de D2. Este concepto es clave para entender cómo las bases de datos combinan múltiples tablas (relaciones) mediante operaciones como el **join**.

Si tenemos tres dominios D1 = {1, 2}, D2 = {"A", "B"} y D3 = {X, Y}, el producto cartesiano sería:

- P = {(1, "A", X), (1, "A", Y), (1, "B", X), (1, "B", Y), (2, "A", X), (2, "A", Y), (2, "B", X), (2, "B", Y)}.

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

## Práctica

### MySQL en Docker con persistencia

#### Creación del contenedor

```bash
# Crear el contenedor
docker run --name mysql-container -e MYSQL_ROOT_PASSWORD=tu_contraseña -e MYSQL_DATABASE=mi_base_de_datos -v mysql_data:/var/lib/mysql -p 3306:3306 -d mysql:latest

# Comprobar que el contenedor está corriendo
docker ps
```

- `--name mysql-container`: Nombre del contenedor.

- `-e MYSQL_ROOT_PASSWORD=tu_contraseña`: Establece la contraseña para el usuario root.

- `-e MYSQL_DATABASE=mi_base_de_datos`: Crea una base de datos inicial llamada mi_base_de_datos.

- `-v mysql_data:/var/lib/mysql`: Crea un volumen llamado mysql_data para persistir los datos.

- `-p 3306:3306`: Expone el puerto 3306 (puerto predeterminado de MySQL) para conectarte desde tu máquina.

- `-d mysql:latest`: Utiliza la imagen más reciente de MySQL y ejecuta el contenedor en segundo plano.

#### Conectarse al contenedor

1. Conectarse desde cualquier cliente MySQL usando `localhost:3306`, el usuario `root` y la contraseña configurada.

2. Conectarse al contenedor de MySQL desde la terminal:

```bash
docker exec -it mysql-container mysql -uroot -p
```

- `docker exec`: Ejecuta un comando en un contenedor en ejecución.

- `-it`: Permite la interacción (interactiva) y asigna un pseudo-TTY.

- `mysql-container`: Nombre del contenedor que especificaste al crear el contenedor.

- `mysql`: Llama al cliente de MySQL.

- `-uroot`: Especifica que te conectas con el usuario root.

- `-p`: Te pedirá que ingreses la contraseña del usuario root (la que configuraste al crear el contenedor).

#### Reiniciar y parar el contenedor

```bash
# Reiniciar el contenedor
docker start mysql-container

# Parar el contenedor
docker stop mysql-container
```

### PostgreSQL en Docker con persistencia

#### Creación del contenedor

```bash
docker run --name postgres-container -e POSTGRES_PASSWORD=tu_contraseña -e POSTGRES_DB=mi_base_de_datos -v postgres_data:/var/lib/postgresql/data -p 5432:5432 -d postgres:latest
```

- `--name postgres-container`: Nombre del contenedor.

- `-e POSTGRES_PASSWORD=tu_contraseña`: Establece la contraseña para el usuario postgres.

- `-e POSTGRES_DB=mi_base_de_datos`: Crea una base de datos inicial llamada mi_base_de_datos.

- `-v postgres_data:/var/lib/postgresql/data`: Crea un volumen llamado postgres_data para persistir los datos.

- `-p 5432:5432`: Expone el puerto 5432 (puerto predeterminado de PostgreSQL) para conectarte desde tu máquina.

- `-d postgres:latest`: Utiliza la imagen más reciente de PostgreSQL y ejecuta el contenedor en segundo plano.

#### Conectarse al contenedor

Es posible conectarse al contenedor vía el cliente `psql` de PostgreSQL:

```bash
docker exec -it postgres-container psql -U postgres
```

#### Reiniciar y parar el contenedor

```bash
# Reiniciar el contenedor
docker start postgres-container

# Parar el contenedor
docker stop postgres-container
```

---

## Referencias

- <https://dev.mysql.com/doc/>
- <https://www.postgresql.org/docs/>
- <https://wiki.postgresql.org/>

- <https://roadmap.sh/sql>
- <https://www.sqltutorial.org/>
- <https://www.sqlitetutorial.net/>
- <https://datalemur.com/sql-tutorial>
- <https://github.com/XD-DENG/SQL-exercise>
- <https://www.w3schools.com/sql/default.asp>
- <https://www.sqlzoo.net/wiki/SQL_Tutorial>
- <https://sqlbolt.com/>
- <https://bookdown.org/paranedagarcia/database/sql.html>
- <https://thedataschools.com/sql/>
- <https://gestionbasesdatos.readthedocs.io/es/latest/index.html>

## Licencia

[![Licencia de Creative Commons](https://i.creativecommons.org/l/by-sa/4.0/80x15.png)](http://creativecommons.org/licenses/by-sa/4.0/)
Esta obra está bajo una [licencia de Creative Commons Reconocimiento-Compartir Igual 4.0 Internacional](http://creativecommons.org/licenses/by-sa/4.0/).
