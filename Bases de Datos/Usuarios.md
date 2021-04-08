# Usuarios
Todos los comandos listados necesitan una cuenta con los privilegios necesarios.

## Creación
```plsql
CREATE USER name IDENTIFIED BY password;
```

## Permisos
### Inicio de sesión
```plsql
GRANT CREATE SESSION TO name;
```

### Crear tablas
```plsql
GRANT CREATE TABLE TO name;
```

### Asignar espacio
```plsql
ALTER USER name QUOTA n u ON USERS;
```

**n:** número de espacio
**u:** unidad (m -> megas, etc)

### Concatenación
Estos comandos se pueden concatenar de la siguiente forma:
```plsql
CREATE USER name IDENTIFIED BY password QUOTA n u ON USER;
GRANT CREATE SESSION, CREATE TABLE TO name;
```