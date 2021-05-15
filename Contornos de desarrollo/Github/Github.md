# Github

## Configuración
### Nombre y correo
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

## Acceso SSH
```bash
# generar key
ssh-keygen -t rsa

# se añade a github desde la pagina
# se comprueba y se autentica
ssh git@github.com
```

-  se inicia el agente ssh y se añade la key
eval `ssh-agent -s`
ssh-add .ssh/key_rsa

- Se añade a github desde la pagina.

- se comprueba y se autentica
ssh git@github.com

<br>

## Comandos básicos

```bash
git clone	[<opciones>][url]					# Clonar repositorio
git log		[<opciones>][<rango de revisión>]	# Mostrar revisiones
git pull	[<opciones>][<repositorio>			# Actualiza el repositorio local
git push	[<nombre>][<branch>]				# Actualiza repositorio remoto
```

[git-clone](https://git-scm.com/docs/git-clone) [git-log](https://git-scm.com/docs/git-log) [git-pull](https://git-scm.com/docs/git-pull) [git-push](https://git-scm.com/docs/git-push) 

<br>

## Issues
### Cerrar desde commit
Desde un commit podemos interactuar con una issue utilizando una palabra clave y el id de la issue, las palabras clave son:

- close
- closes
- closed
- fix
- fixes
- fixed
- resolve
- resolves
- resolved

#### Ejemplo
`Arreglos closes #31`