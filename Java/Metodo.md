# Método
Es un bloque de codigo que solo se ejecuta cuando es llamado. Puede o no admitir parametros.

## Estructura
Un metodo está compuesto por un modificador de acceso, un [tipo  de dato](Tipo&#32;de&#32;datos.md) a devolver, [nombre del metodo](Identificadores.md###Métodos)  seguido de entre parentesis posibles parametros y el cuerpo entre llaves.

```java
public int suma(int n1, int n2)	{ /* codigo */ }	// devuelve int
public void nada()				{ /* codigo */ }	// no devuelve
```

<<<<<<< HEAD
## Abstractos
=======
## Abstracto
>>>>>>> 17e28880f40ff50ccc22ba7e83c2e7c2a96a5ef7
Es declarado pero no implemenetado.

```java
abstract void mover(float x, float y);
```