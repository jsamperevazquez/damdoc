# XPath
Permite construir expresiones que recorren y procesan un documento XML. Permite buscar y seleccionar teninedo en cuenta la estructura jerárquica del XML.

## Tipos de Nodos
### Raíz
Se identifica por `/`. No confundir con el elemento reíz del documento.


### Elemento
Cualquier elemento de un documento XML se convierte en un nodo elemento dentro del árbol.


### Texto
Todos los caracteres del documento que no están marcados con alguna etiqueta.


### Atributo
Consta de un nombre, un valor y un posible "espacio de nombres".


### Comentario e instrucciones de proceso
También se generan nodos para cada cometnario e instrucciones de proceso.


## Sintaxis
### Selección
| Expresión | Descripción                                           |
| --------- | ----------------------------------------------------- |
| /         | Selecciona desde el nodo raiz                         |
| //        | Selecciona nodos en el documento desde el nodo actual |
| .         | Selecciona el nodo actual                             |
| ..        | Selecciona el nodo padre del nodo actual              |
| @         | Selecciona atributos                                  |
| text()    | Selecciona el contenido del elemento                  |
| *         | Selecciona cualquier nodo                             |
| @*        | Selecciona cualquier atributo                         |
| node()    | Selecciona cualquier nodo                                                      |


### Predicados
Permiten encontrar un nodo específico o un nodo que contiene un valor específico.

| Expresión      | Resultado                                           |
| -------------- | --------------------------------------------------- |
| [1]            | Selecciona el primer elemento hijo                  |
| [last()]       | Selecciona el último elemento hijo                  |
| [last()-1]     | Selecciona el elemento anterior al ultimo hijo      |
| [position()<3] | Selecciona los dos primeros elementos hijo          |
| [@lang]        | Selecciona todos los elementos con el atributo lang |


### Ejes
Define el conjunto de nodos relativos al nodo actual

| Nombre             | Resultado                                                                           |
| ------------------ | ----------------------------------------------------------------------------------- |
| ancestor           | Selecciona todos los nodos antecesores                                              |
| ancestor-or-self   | Selecciona todos los nodos antecesores y el actual                                  |
| attribute          | Selecciona todos los atributos                                                      |
| child              | Selecciona todos los hijos                                                          |
| descendant         | Selecciona todos los nodoso descendentes                                            |
| descendant-or-self | Selecciona todos los nodos descendientes y tambien el actual                        |
| following          | Selecciona todo en el documento a partir de la etiqueta de cierre                   |
| following-sibling  | Selecciona todos los hermanos                                                       |
| parent             | Selecciona el padre                                                                 |
| preceding          | Selecciona todo en el documento que está antes de la etiqueta del comienzo del nodo |
| preceding-sibling  | Selecciona todos los nodos hermanos antes del nodo actual                           |
| self               | Selecciona el nodo actual                                                           | 


### Localización
Una ruta puede ser absoluta o relativa. Las rutas absolutas comienzan con `/`, las absolutas no.


### Operadores

| Operador | Descripción                    | Devuelve                  |
| -------- | ------------------------------ | ------------------------- |
|          | Calcula dos conjuntos de nodos | Conjunto de los elementos |
| +        | Adición                        | Resultado                 |
| -        | Sustracción                    | Resultado                 |
| *        | Multiplicación                 | Resultado                 |
| div      | División                       | Resultado                 |
| =        | Igualdad                       | Verdadero/Falso           |
| !=       | Distinto                       | Verdadero/Falso           |
| <        | Menor que                      | Verdadero/Falso           |
| <=       | Menor o igual                  | Verdadero/Falso           |
| >        | Mayor que                      | Verdadero/Falso           |
| >=       | Mayor o igual                  | Verdadero/Falso           |
| or       | o                              | Verdadero/Falso           |
| and      | y                              | Verdadero/Falso           |
| mod      | Resto de la división           | Resultado                 |


### Funciones

#### Numericas

| Función      | Descripcción                                              |
| ------------ | --------------------------------------------------------- |
| number(arg)  | Devuelve el valor numerico del argumento                  |
| abs(arg)     | Devuelve el valor absoluto del argumento                  |
| ceiling(arg) | Devuelve el valor integer superior al argumento           |
| floor(arg)   | Devuelve el valor integer inferior al argumento           |
| round(arg)   | Devuelve el valor integer redondeado al valor más proximo | 

#### Agregado

#### Cadena