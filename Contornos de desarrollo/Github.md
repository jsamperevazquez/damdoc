# Github

## Comandos

### Configuración
#### Nombre y correo
Para configurar el nombre que se mostrará y el correo electronico se usa:

```bash
git config --global user.name "Nombre"
git config --global user.email ejemplo@mail.ru
```
[Git - First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) [Git - git-config](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

<br>

#### Contraseña
En determinadas acciones se requiere introducir una contraseña, para guardarla temporalmente al inicio de la sesión y así no tener que introducirla cada vez se puede usar:

```bash
git config --global credential.helper 'cache --timeout=36000'	# 1 hora
```
[Git Tools - Credential Storage](https://git-scm.com/book/fa/v2/Git-Tools-Credential-Storage)

<br>

#### Editor predeterminado

```bash
git config --global core.editor [directorio]
```

<br>

#### Comandos básicos

```bash
git clone	[<opciones>][url]					# Clonar repositorio
git log		[<opciones>][<rango de revisión>]	# Mostrar revisiones
git pull	[<opciones>][<repositorio>			# Actualiza el repositorio local
git push	[<nombre>][<branch>]				# Actualiza repositorio remoto
```

[git-clone](https://git-scm.com/docs/git-clone) [git-log](https://git-scm.com/docs/git-log) [git-pull](https://git-scm.com/docs/git-pull) [git-push](https://git-scm.com/docs/git-push) 

## SSH
```bash
# generar key
ssh-keygen -t rsa

# se inicia el agente ssh y se añade la key
eval `ssh-agent -s`
ssh-add .ssh/key_rsa

# se añade a github desde la pagina

# se comprueba y se autentica
ssh git@github.com
```

## Issues
### Cerrar
Los Issues se pueden cerrar de dos formas:
+ Cerrando en los comentarios.
+ Mediante un commit, añadiendo al final o al principio una palabra clave y el id, ej: ```resolves #10804```

Las palabras clave son:

```
close, closes, closed, fix, fixes, fixed, resolve, resolves, resolved
```

## Proyecto
### Kanban
Puede automatizar las [issues](Contornos&#32;de&#32;desarrollo/Github.md#issues).