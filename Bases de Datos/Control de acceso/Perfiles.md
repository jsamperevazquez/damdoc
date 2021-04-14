# Perfiles
## Creación
```plsql
CREATE_PROFILE name
LIMIT SESSIONS_PER_USER n
CONNECT_TIME n
IDLE_TIME n
PASSWORD_LOCK_TIME n
PASSWORD_LIFE_TIME n
PASSWORD_GRACE_TIME n;
```

## Asignación
```plsql
-- creación de perfil y asignación
CREATE USER name
IDENTIFIED BY password
QUOTA n m
ON tablespace
PROFILE profile;
```