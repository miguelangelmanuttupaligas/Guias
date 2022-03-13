# Guía SQL Server - Básica

Convenciones de sintaxis de Transact-SQL : https://docs.microsoft.com/es-es/sql/t-sql/language-elements/transact-sql-syntax-conventions-transact-sql?view=sql-server-ver15


Convención | Uso
--- | --- 
MAYÚSCULAS | Palabras clave
*cursiva* | Parámetros dados por usuario
**Negrita** | Nombres de variables ya establecidas(bases de datos,tablas,columnas,etc.)
(barra vertical) | Separa los elementos de sintaxis escritos, ubicados entre corchetes o llaves
[ ] | Elementos opcionales de sintaxis
{ } | Elementos obligatorios de sintaxis
[, ...n] | Elemento anterior puede repetirse *n* veces. Se separan por comas 
[...n] | Elemento anterior puede repertirse *n* veces. Se separan por espacios en blanco
; | Terminador de instrucción de Transacat-SQL
 `<label>::=` | Nombre de un bloque de sintaxis. 

## Crear una base de datos

```sql
CREATE DATABASE database_name
```

## Crear una tabla

```sql
CREATE TABLE table_name(
    col1_name varchar(45),
    col2_name varchar(45)
) 
```

## Visualizar tablas y columnas
### Visualizar tablas de una base de datos
```sql
EXEC sp_tables @table_owner='dbo';
```
### Visualizar columnas de una tabla
```sql
EXEC sp_columns table_name
```

## Insertar datos en tablas
```sql
INSERT INTO table_name(col1,col2) VALUES('value1','value2')
```
## Seleccionar datos de tablas
```sql
SELECT col1,col2 FROM table_name
```
## Tipos de datos en SQL Server
### Numéricos exactos
- bigint
- bit 
- decimal 
- int 
- money 
- numeric 
- smallint 
- smallmoney 
- tinyint
### Numéricos aproximados
- float
- real
### Fecha y hora
- date
- datetime2
- datetime
- datetimeoffset
- smalldatetime
- time
### Cadenas de caracteres
- char
- varchar
- text
### Cadenas de caracteres Unicode
- nchar
- nvarchar
- ntext
### Cadenas binarias
- binary
- image
- varbinary
### Otros tipos de datos
- cursor
- rowversion
- hierarchyid
- uniqueidentifier
- sql_variant
- xml
- Tipos de geometría espacial
- Tipos de geografía espacial
- table

## Cláusula SELECT
```sql
SELECT select_list 
[INTO new_table] 
[FROM table_source] 
[WHERE search_condition] 
[GROUP BY group_by_expression] 
[HAVING search_condition] 
[ORDER BY order_expression [ASC|DESC]] 
```
### Orden de procesamiento lógico de la instrucción SELECT
- FROM
- ON
- JOIN
- WHERE
- GROUP BY
- WITH CUBE o WITH ROLLUP
- HAVING
- SELECT
- DISTINCT
- ORDER BY 
- TOP

### Ejemplos de SELECT
Consulte la documentación aquí: https://docs.microsoft.com/es-es/sql/t-sql/queries/select-examples-transact-sql?view=sql-server-ver15

## Operadores
### Aritméticos
`+`, `-`, `*`, `/` y `%`
### Asignación
`=` Único operador de asignación de Transact-SQL
### Bit a Bit
Operador | Uso
--- | --- 
y |Si los dos bits, en cualquier ubicación, son 1, el resultado es 1.
O |Si cualquiera de los dos bits, en cualquier ubicación, es 1, el resultado es 1.
NOT |Invierte el valor de bit en cada ubicación de bits.	1010 1010 = 170

0101 0101 = 85
### Comparación
Operador | Uso
--- | --- 
`=` |(Es igual a)	Igual a
`>` |(Mayor que)	Mayor que
`<` |(Menor que)	Menor que
`>=` |(Mayor o igual a)	Mayor o igual que
`<=` |(Menor o igual a)	Menor o igual que
`<>` |(No es igual a)	No es igual a
`!=` |(No es igual a)	No es igual a (no es del estándar ISO)
`!<` |(No menor que)	No es menor que (no es del estándar ISO)
`!>` |(no mayor que)	No es mayor que (no es del estándar ISO)
### Compuestos
Operador | Uso
--- | --- 
+=	| Agrega una cantidad al valor original y establece este en el resultado de la operación.
-=	| Resta una cantidad del valor original y establece este en el resultado de la operación.
*=	| Multiplica por una cantidad y establece el valor original en el resultado de la operación.
/=	| Divide por una cantidad y establece el valor original en el resultado de la operación.
%=	| Divide por una cantidad y establece el valor original en el módulo.
&=	| Realiza una operación AND bit a bit y establece el valor original en el resultado de la operación.
^=	| Realiza una operación OR exclusiva bit a bit y establece el valor original en el resultado de la operación.
|=	| Realiza una operación OR bit a bit y establece el valor original en el resultado de la operación.
### Lógicos
Operador | Uso
--- | --- 
ALL	| TRUE si el conjunto completo de comparaciones es TRUE.
AND	| TRUE si ambas expresiones booleanas son TRUE.
ANY	| TRUE si cualquier miembro del conjunto de comparaciones es TRUE.
BETWEEN	| TRUE si el operando está dentro de un intervalo.
EXISTS	| TRUE si una subconsulta contiene cualquiera de las filas.
IN	| TRUE si el operando es igual a uno de la lista de expresiones.
LIKE	| TRUE si el operando coincide con un patrón.
NOT	| Invierte el valor de cualquier otro operador booleano.
OR	| TRUE si cualquiera de las dos expresiones booleanas es TRUE.
SOME	| TRUE si alguna de las comparaciones de un conjunto es TRUE.
### Relacionales
Operador | Uso
--- | --- 
OPENDATASOURCE
OPENQUERY
OPENROWSET
OPENXML
OPENJSON 
PREDICT
STRING_SPLIT
### Resolución de ámbito
`::` Proporciona acceso a los miembros estáticos de un tipo de datos compuesto.

### Conjuntos
Operador | Uso
--- | --- 
EXCEPT | devuelve filas distintas de la consulta de entrada izquierda que no son de salida en la consulta de entrada derecha.
INTERSECT | devuelve filas distintas que son el resultado del operador de las consultas de entrada izquierda y derecha.
UNION | Concatena los resultados de dos consultas en un único conjunto de resultados. Puede controlar si en el conjunto de resultados se incluyen filas duplicadas:
### Concatenación de cadenas
Operador | Uso
--- | --- 
`+` | Concatenación de cadenas
`+=` | Concatenación de cadenas y asignación
`%` | Comodín - Caracteres para coincidir
`[]` | Caracteres comodín para coincidencia
`[^]` | Caracteres comodín para no coincidencia
`_` | Comodín - Un carácter para coincidir
### Unarios
Operador | Uso
--- | --- 
`+` | El valor numérico es positivo.
`-` | El valor numérico es negativo.
`~` | Devuelve los bits complementarios del número.