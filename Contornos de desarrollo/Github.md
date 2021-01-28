# Github

## Comandos

### Configuración
#### Nombre y correo
<div style="text-align: justify;">
	Para configurar el <span style="color: #A6E22E;">nombre</span> que se mostrará y el <span style="color: #A6E22E;">correo electronico</span> se usa:
</div>

```bash
git config --global user.name "Nombre"
git config --global user.email ejemplo@mail.ru
```
[Git - First-Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) [Git - git-config](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

<br>

#### Contraseña
<div style="text-align: justify;">
	En determinadas acciones se requiere introducir una contraseña, para guardarla temporalmente al inicio de la sesión y así no tener que introducirla cada vez se puede usar:
</div>

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

# se añade a github desde la pagina
# se comprueba y se autentica
ssh git@github.com
```