# Programación estructurada
Es un método estandarizado de resolución de algoritmos basados en el teorema de estructura. Todos los programas pueden ser escritos utilizando tres tipos de estructura.

## Estructuras de control

### Secuencial
Se compone de una serie de procesos que se ejecutan uno a continuación de otro sin repetir ninguno y sin omitir ni bifurcar.

### Condicional
Permite elegir que ejecutar según una o varias condiciones. Hay varios tipos.

#### Simples
Si se cumple la condición se ejecuta una serie de instrucciones, de lo contrario se obvian.

```java
if (condition) {
	// código
}
```

#### Dobles
Permite elegir entre dos opciones posibles en función del cumplimiento o no de la condición.

```java
if (condition) {
	// se cumple
} else {
	// no se cumple
}
```

Alternativa:

```java
String color = (condition) ? "blanco": "negro";
```

#### Múltiples
Son tomas de decisión especializadas que permiten comparar una variable contra distintos posibles resultados, ejecutando para cada caso una serie de instrucciones especificas.

```java
if (condition0) {
	// se cumple
} else {
	// no se cumple

	if (condition1) {
		// se cumple
	} else {
		// no se cumple
		// ...
	}
}
```

Alternativamente se puede usar:

```java
switch (condition) {
	case 0:
		// ...
		break;
	
	case 1:
		// ...
		break;
	
	case 2:
		// ...
		break;
	
	default:
		break;
}
```


### Repetitiva
Permite repetir una o un grupo de sentencias varias veces. Este conjunto de sentencias se denomina bucle. Hay varios tipos de bucle:

#### do-while
Se ejecuta el código y luego comprueba si la condición se cumple, mientras esta se cumpla se seguirá ejecutando.

```java
do {
	// código
} while (condition)
```

#### while
Comprueba si se cumple una condicíon y ejecuta el código mientras esta se cumpla.

```java
while (condition) {
	// código
}
```

#### for
Ejecutar un código un número de veces concretas. Se utiliza el [identificador](Identificadores.md###Variables ) i por convenio.

```java
for (int i = 0; i < 10; i++) {
	// código
}
```

#### for-each
Ejecuta un código tantas veces como elementos haya en una colección.

```java
String[] colors = {"red", "green", "blue"};

for (String i : colors) {
	// código
}
```
