# Interfaz
Es una colección de métodos abstractos y propiedades constantes.

## Ejemplo
```java
public interface IPoligono {
	...
}

public class Rectangulo implements IPoligono {
	private float base;
	private float altura;
	
	// constructor, getters, setters
	
	public float calcularArea() {
		return (base * altura);
	}
	
	public float calcularPerimetro() {
		return (2 * base + 2 * altura);
	}
}
```