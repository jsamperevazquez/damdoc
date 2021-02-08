# XML
Es un meta-lenguaje que permite crear etiquetas adaptadas a las necesidades. El estándar define cómo pueden ser esas etiquetas y qué se puede hacer con ellas. Es además especialmente estricto en cuanto a lo que está permitido yl o que no, todo el documento debe cumplir dos condiciones: ser válido y estar bien formado.

Este tipo de codificación permite interpretarla directamente, dado que son archivos de texto plano. Al tratarse solamente de texto, los documentos son independientes de la plataforma, sistema o programa con el que fueron creados.

## Estructura
Todos los documentos XML deben empezar con:

```xml
<?xml version="1.0" encoding="UTF-8">
```

Esta linea define:
+ `version`, describe la versión y es obligatorio a no ser que sea un documento externo a otro que ya lo incluya.
+ `encoding`, describe la forma en la que se ha codificado el documento y depende el interprete el entender o no la codificación.
+ `standalone`, indica si el documento va acompañado de un DTD ("no"), o no lo necesita ("yes"), este atributo es opcional.

