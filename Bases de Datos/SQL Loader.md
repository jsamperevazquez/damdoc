# SQL Loader
Permite cargar datos de archivos en tablas.

## Cargar datos
Para cargar los datos debemos hacer un archivo `.ctl`

### Fijos
```plsql
LOAD DATA
INFILE file_name
INTO TABLE table_name
APPEND 
TRAILING NULLCOLS (
	field_name_0 POSITION(X:Y),
	field_name_1 POSITION(X:Y),
	field_name_2 POSITION(X:Y),
	field_name_3 POSITION(X:Y),
	field_name_4 POSITION(X:Y) "TO_DATE(:datan, 'DDMMYYYY')"
)
```

### Relativos
```plsql
LOAD DATA
INFILE file_name
INTO TABLE table_name
APPEND 
FIELDS TERMINATED BY ','
TRAILING NULLCOLS (
	field_name_0,
	field_name_1,
	field_name_2,
	field_name_3,
	field_name_4 "TO_DATE(:datan, 'DDMMYYYY')"
)
```

Desde la terminal cargamos el archivo:
```bash
sqlldr user/password control = file_name
```