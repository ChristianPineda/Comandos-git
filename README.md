### Comandos de GIT y Terminal
============

*Una pequeña lista de los comandos mas utilizados en Git y la Terminal*

--

### Comandos de la Terminal

| Command | Descripción |
| -------| ------------ |
| `cd [rute]`| Cambia el directorio |
| `mkdir [name]` | Crea una nueva carpeta |
| `ls -a`| Lista los archivos del directorio |
| `clear`| Limpia la Terminal |
| `Touch [name.txt]`| Crea un archivo vacio |
| `rm [file]`| Elimina un archivo |
| `rm -rf [dir]`| Elimina una carpeta |
| `pwd`| Muestra el directorio donde nos encontramos |
| `mv`| Mueve o renombra archivos |
| `cat [name.txt]`| Vista previa del contenido del archivo |
| `sudo`| Ejecuta un commando como administrador |

### Configuracion de Git

| Command| Descripción |
| -------| ------------ |
| `git config --global user.name "name-example"`| Añade un nombre de usuario |
| `git config --global user.email user@example.com`| Añade un correo del usuario |
| `git config --list`| Muestra todas las configuraciones |

### Config SSH Keys / Configuracion de Credenciales SSH

| Command| Descripción |
| -------| ------------ |
| `ssh-keygen -t rsa -b 4096 -C "Email"`| Generar credencial SSH |
| `eval $(ssh-agent -s)`| Verifica la existencia del servidor de credenciales SSH |
| `ssh-add [rute]`| Agrega la credencial SSH al entorno de trabajo |

### Creacion de proyectos

| Command| Descripción |
| -------| ------------ |
| `git init`| Inicia un repositorio local de Git |
| `git clone [url]`| Crea una copia local de un repositorio remoto |

### Snapshooting Basico

| Command| Descripción |
| -------| ----------- |
| `git status`| Verifica el estatus del repositorio |
| `git add [file-name.txt]`| Añade un archivo al area de preparación |
| `git add .`| Añade todos los archivos al area de preparación |
| `git commit -m "[commit message]"`| Añade los archivos al repositorio |
| `git commit -am "[commit message]"`| Añande los cambios y hace commit |
| `git rm -r [file-name.txt]`| Elimina archivos o carpetas |
| `git commit --ammend`| Agrega los cambios al ultimo commit en caso de error |

### Ramas y fusionar

| Command| Descripción |
| -------| ----------- |
| `git branch`| Lista todas las ramas |
| `git branch -a`| Lista todas las ramas locales y remotas |
| `git branch [branch name]`| Crea una nueva rama |
| `git branch -d [branch name]`| Elimina una rama |
| `git show-branch --all`| Lista todas las ramas en local |
| `git push origin --delete [branch name]`| Elimina una rama remota |
| `git checkout -b [branch name]`| Crea una nueva rama y cambia a ella |
| `git checkout -b [branch name] origin/[branch name]`| Clona una rama remota y cambia a ella |
| `git checkout [branch name]`| Cambiar a una rama determinada |
| `git checkout -`| Cambia a la ultima rama seleccionada |
| `git checkout -- [file-name.txt]`| Descarta los cambios de un archivo |
| `git merge [branch name]`| Fusiona una rama a la rama activa
| `git merge [source branch] [target branch]`| Fusiona una rama a una rama determinada |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Compartiendo y Repositorios Remotos

| Command| Descripción |
| -------| ----------- |
| `git push origin [branch name]`| Envia el repositorio local a remoto |
| `git push origin --delete [branch name]`| Elimina un repositorio remoto |
| `git pull`| Envía actualizaciones al repo remoto, puedes añadir un archivo o una rama solamente, o simplemente "pull" para agregar todo
| `git pull origin [branch name]`| Hace un feth y fusiona
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git`| Crea un repositorio remoto |
| `fork`| Copa un repositorio externo |
| `git remote -v`| Lista las conexiones remotas |
| `git remote set-url [branch name] [url]`| Cambia la url del repositorio |

### Inspeccion y Comparacion

| Command| Descripción |
| -------| ----------- |
| `git log`| Muestra los cambios en el repositorio |
| `git log --summary`| Muestra los cambios en el repositorio detalladamente |
| `git log -all --graph --decorate --oneline`| Muestra todos los cambios del repositorio detallada y graficamente |
| `git diff [source branch] [target branch]`| Compara los diferentes cambios |


### Otros

| Command| Descripción |
| ------- | ----------- | ----------- |
| `alias [name=] "command"`| Crea un alias para llamar a un comando |
| `git tag -a [name] -m "message" [id/hashtag]`| Crea un tag de un commit en especifico |
| `git show-ref --tags`| Lista los tags existentes |
| `git push --tags`| Envia los tags al repositorio remoto |
| `git tag -d [name]`| Elimina un tag en especifico |
| `git push origin :refs/tags/[name]`| Elimina un tag dentro de GitHub |
| `gitk`| Abre una interfaz grafica |
| `git cherry.pick [id]`| Trae un commit especifico desde otra rama |
| `git grep -n [word]`| Busca la palabra especificada en todo el proyecto |
