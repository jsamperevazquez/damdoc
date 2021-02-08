# Constructor
[Método](M%C3%A9todo.md) especial usado para inicializar un objeto, es llamado cuando una clase es creada y permite establecer valores para los atributos del objeto.

Este metodo se llama igual que la clase y no puede devolver nada, en caso de no ser declarado Java creará uno por defecto.

```java
public class NombreClase {
	int entero;					// Crea atributo

	public NombreClase() {
		entero = 0;				// Inicializa atributo
	}
}
```