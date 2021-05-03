# expdp & impdp
Nos permite exportar e importar tablas, desde una terminal donde previamente hayamos iniciado el entorno de Oracle.

## expdp
Para exportar datos, previamente tenemos que hacer un archivo de configuración.

`expdp user/pass PARFILE = configuration.txt`

### Configuración

```plsql
-- directorio base
directory=dir

-- archivo que contiene las tablas
dumpfile = file.dmp

-- tablas a cargar
tables = table0, table1

```

## impdp
Para importar datos, previamente tenemos que hacer un archivo de configuración.

`impdp user/pass PARFILE = configuration.txt`

### Configuración

```plsql
-- directorio base
directory = dir

-- archivo que contiene las tablas
dumpfile = file.dmp

-- tablas a cargar
tables = table0, table1

-- si la tabla existe
-- se añaden los datos
table_exists_action = append

-- solo las tablas que contengan...
query=table0:"WHERE key = 'value'"
```