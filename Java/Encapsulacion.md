# Encapsulación
Permite ocultar los datos sensibles, principalmente de accesos no deseados. Para ello se debe:
+ Declarar como privadas las variables de clase.
+ Proporcionar métodos públicos GET/SET para acceder y actualizar los atributos privados.

## Get/Set
Dado que solo se puede acceder a las variables privadas desde dentro de la misma clase, se utilizan dos metodos, get y set.
```java
public class Persona {
	private String nombre;
	
	// Getter
	public String getNombre() {
		return nombre;
	}

	// Setter
	public void setNombre(String nuevoNombre) {
		this.nombre = nuevoNombre;
	}
}
```
