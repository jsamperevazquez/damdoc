# Tipo de datos
## Primitivos
Podríamos considerarlos fundamentales, ya que la mayor parte de los demás tipos, los estructurados o complejos, son composiciones a partir de estos más básicos.

<br>

### Números enteros
| Tipo  	|  Tamaño 	| Mínimo               	| Máximo              	|
|-------	|:-------:	|----------------------	|---------------------	|
| byte  	|  1 byte 	| -128                 	| 127                 	|
| short 	| 2 bytes 	| -32768               	| 32768               	|
| int   	| 4 bytes 	| -2147483648          	| 2147483647          	|
| long  	| 8 bytes 	| -9223372036854775808 	| 9223372036854775807 	|

### Números de punto flotante
| Tipo   	|  Tamaño 	| Decimales 	| Mínimo                	| Máximo               	|
|--------	|:-------:	|:---------:	|-----------------------	|----------------------	|
| float  	| 4 bytes 	|     ~7    	| -3.402823e38          	| 3.402823e38          	|
| double 	| 8 bytes 	|    ~16    	| -1.79769313486232e308 	| 1.79769313486232e308 	|

### Booleanos y caracteres
| Tipo    	|  Tamaño 	| Descripción                                             	|
|---------	|:-------:	|---------------------------------------------------------	|
| boolean 	|  1 bit  	| false/true                                              	|
| char    	| 2 bytes 	| Almacena un solo carácter, puede ser en forma númerica. 	|

<br>

## Estructurados
Los tipos de datos estructurados o tipos compuestos son agrupaciones de otros tipos de datos.

<br>

### Cadena de caracteres
Una cadena de caracteres es una secuencia de caracteres que está tratada como un unico dato.

<br>

### Vector
Permite agrupar variables de un mismo tipo con un único nombre.

<br>

### Matriz
Es el resultado de crear un vector utilizando como base otro vector.

<br>

## Avanzados
### Estructura de datos
#### Arrays
+ Fáciles
+ Permite almacenar datos primitivos y estructurados.
+ Gestión de memoria estática
+ Solo permite datos del mismo tipo

Es un conjunto primitivo del mismo tipo que ocupan posiciones consecutivas de memoria.

##### Declaración
```java
tipo[] nombreArray;
tipo nombreArray[];
```

#### Colecciones
+ Complejas
+ Permite almacenar datos estructurados
+ Gestión de memoria dinámica

##### List
+ Admite repeticiones


##### Set
+ No admite repeticiones

##### Map
+ Almacena datos en parejas *key-value*
