# Roles
Permite agrupar privilegios para posteriormente darselos a un [usuario](Usuarios.md).

## Creación
Es necesario tener el permiso `CREATE ROLE`.

```plsql
CREATE ROLE name;
```


## Asignar privilegios

```plsql
-- privilegios de sistema
GRANT privilege,... TO name WITH ADMIN OPTION;

-- privilegios de objeto
GRANT privilege,... TO schema_name.object_name TO name;
```