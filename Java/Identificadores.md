# Identificadores
Los identificadores son nombres que se asignan a variables, constantes, clases métodos, paquetes...

## Reglas
+ Los unicos caracteres permitidos son los alfanuméricos ([AZ], [az], [0-9]), '_' y '$' .
+ No deben empezar con dígitos.
+ Los identificadores distinguen entra mayúsculas y minúsculas.
+ La longitud óptima es de 4 a 15 caracteres, pero no hay limite.
+ Las [palabras clave](Palabras&#32;reservadas.md) no se pueden usar como un identificador.

<br>

## Convenio
Es importante usar unas normas de codificación claras y homogéneas para que cualquiera pueda entenderlas, ya que facilitan la legibilidad del código.

<br>

### Clases e Interfaces
La primera letra de cada palabra debe estar en mayúscula. En el caso de las clases, el nombre debe ser descriptivo, usando un sustantivo o adjetivo.

### Métodos
Deben ser verbos, utilizando mayúsculas y minúsculas, siendo la primera letra de cada palabra interna (a partir de la segunda) en mayúscula.

### Variables
+ Debe ser cortos y significativos.
+ Debe ser mnemotécnico, es decir, debe indicar al observador casual la intención de su uso.
+ Se deben evitar los nombres de un carácter, excepto para varaibles temporales.
+ Los nombres comunes para las variables temporales son:
	+ Enteros: i, j, k, m, n.
	+ Caracteres: c, d, e.

### Constantes
Debe estar todo en mayúsculas con palabras separadas por guiones bajos.

### Paquetes
El prefijo de un nombre de paquete único siempre se escribe en letras ASCII en minúsculas y debe ser uno de los nombre de dominio de nivel superior. Los componentes posteriores del nombre del paquete varían de acuerdo con las convenciones internas de nombres de la organización.