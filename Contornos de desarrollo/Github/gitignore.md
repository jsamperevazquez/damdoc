# .gitignore

Permite ignorar archivos a la hora de hacer commits.


## Que ignorar

- Archivos log.
- Archivos con claves o información sensible.
- Archivos inútiles como `.DS_STORE` en macOS.
- Archivos generados, como la carpeta `/dist`.
- Otros archivos irrelevantes como configuraciones del IDE o listas TO DO.


## Funcionamiento

Es un archivo de texto plano en que cada linea define un patrón para ignorar archivos o directorios. Generalmente el archivo `.gitignore` se situa en el directorio raiz del repositorio y puede haber varios.


### Nombres literales

La forma más fácil de definir uno de estos patrones es escribir el nombre literal:

```
.DS_Store
```


### Directorios

Para ignorar un directorio entero solo hay que incluir `/` al final:

```
node_modules/
logs/
```


### Comodín

Usando `*` haremos referencia a 0 o más caracteres, excepto `/`. Por ejemplo, usando `*.log` coincidirá con cualquier archivo con extensión `.log`.

Otro ejemplo es `*~`, que incluirá cualquier archivo terminado en `~`.

Además también se puede usar `?`, el cual hace referencia a cualquier caracter excepto `/`.


### Negación

Usando `!` negamos un archivo que sería excluido.

```
*.log
!example.log
```

Esto permite ignorar todos los archivos `.log` excepto `example.log`.

No se pueden negar archivos que se encuentren dentro de un directorio ignorado.


### Doble asterisco

Permite incluir cualquier numero de directorios.

- `**/logs` incluye todos los archivos o directorios que se llamen `logs`.
- `**/logs/*.log` incluye todos los archivos con extensión `.log` de cualquier carpeta `logs`.

También permite incluir cualquier todos los archivos de un directorio:

```
logs/**
```


### Comentarios

Todas las lineas que comiencen por `#` son comentarios:

```
# macOS files
.DS_Store
```


## Reglas personales

Dado que este archivo afecta a todo el repositorio, hay algunas opciones para ignorar archivos sin cambiar el `.gitignore`. Puede que trabajes en unos archivos del proyecto que no quieres incluir o uses un editor distinto al de tus compañeros y siempre quieras excluir unos archivos.


### Reglas locales

Para ignorar archivos en el **repositorio local** hay que añadir las reglas al archivo `.git/info/exclude`.


### Reglas globales

Para ignorar archivos en **todos los repositorios** en tu ordenador primero debes configurar git con:

``` bash
git config --global core.excludesFile ~/.gitignore
```

Y luego podrás añadir las reglas globales a `~/.gitignore`.


## Ignorar un archivo ya en remoto

Git no ignorará un archivo que ya esté en el repositorio remoto, por lo que debes eliminarlo primero para que deje de "seguirlo".

``` bash
git rm --cached FILENAME
```


## Debugging

Puedes ver que archivos están siendo ignorados usando el comando:

```
git check-ignore -v FILENAME
```

Que nos devolverá algo similar a:

```
.gitignore:1:*.log       example.log
```

Lo que significa que el archivo `example.log` está siendo ignorado por el archivo `.gitignore` con el patrón `*.log`.

<br>


## Plantillas

Existen plantillas predefinidas según el IDE, lenguaje, sistema operativo...

- [gitignore.io](https://www.toptal.com/developers/gitignore)
- [github/gitignore](https://github.com/github/gitignore)


<br>

##### Fuentes

- [Pluralsight](https://www.pluralsight.com/guides/how-to-use-gitignore-file)