# Clases
Es un tipo definido por el programador que describe los atributos y los métodos de los objetos que se crean a partir de ella.

```java
/* modificador acceso class Nombre */

public static class NombreClase {}
```

Variables:
+ Instancia: son atributos de objeto.
+ Clase: pertenecen a la clase y son comunes a todas las instancias.
+ Locales: se declaran en los métodos o estructuras.
+ Parametros: se declaran en los parentesis de los métodos. Son variables de enlace entre llamadas.

Constantes:
+ Variable/Atributo.
+ Método: permite deshabilitar el sobreescribir.
+ Clase: deshabilita la herencia.

Métodos:
+ Constructores.
+ Acceso.
+ Sobreescritura (@override).

## Abstracta
No se instancia, pero si se declara y generalmente tiene algun metodo abstracto.

## Internas
Son clases definidas dentro de otras y tienen acceso a los métodos y variables de la externa.