# Limitación de recursos
## Aplicar limitación
```plsql
ALTER SYSTEM SET RESOURCE_LIMIT = TRUE SCOPE=scope;

/*
 * scope
 *
 * MEMORY 	Aplicación inmediata, temporal (hasta reinicio).
 * SPFILE	Aplicación en el arranque, permanente.
 * BOTH		Ambas.
 */
```