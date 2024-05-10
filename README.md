# COMANDOS DE GIT

Git es un sistema de control de versiones o VCS (Version Control System) que ayuda a los equipos de desarrollo a gestionar los cambios en el código fuente a lo largo del tiempo. Este sistema nos permite almacenar un histórico de la evolución del desarrollo y nos ayuda al control de conflictos cuando hay varias personas trabajando sobre el mismo fichero.


#### Contenidos del artículo

#### 1.- Git y repositorios

* git --version  # Ver la versión de Git y comprobar si está instalado

* git config --global user.name [nombre]  # Definir nombre usuario

* git config --global user.email [email]  # Definir email

* git init  # Crear un repositorio en la carpeta actual

* git clone [url-repository]  # Crear un repositorio basado en un repositorio remoto

* git clone [url-repository] .  # Al añadir un punto al final, el clonado se hace en la carpeta donde lanzamos la orden sin crear una subcarpeta.

#### 2.- Estados y consultas

* git status  # Lista de archivos modificados con su estado

* git log  # Muestra todos los commits de la rama actual

* git log --oneline  # Muestra todos los commits (primera línea)

* git checkout [identificador-commit] # Ver un commit mediante su identificador

* git reflog  # Lista ordenada de los commits realizados. Este historial nos sirve para deshacer cambios en el repositorio.

* git checkout --  # Volver al estado original. Reemplaza los cambios en tu directorio de trabajo con el último contenido de HEAD

* git commit --amend -m “message” # Reemplazar un commit

*git restore --staged <file-name> # Eliminar un archivo del stage

#### 3.- Commits

* git add [file-name]  # Agregar el archivo seleccionado al stage 

* git add .  # Agregar todos los archivos modificados al stage

* git reset  # Deshacer los cambios locales en el estado de un repositorio de Git. Por ejemplo: Descartar commits en una rama o descartar cambios no commiteados 

* git reset [file-name]  # Descartar un archivo del stage 

* git commit -m "[description]"  # Crear un commit de los archivos en stage, con una descripción breve

* git commit -am "[description]"  # Crear un commit de los archivos en seguimiento, con una descripción breve

* git push origin [branch] # Subir al repositorio los cambios de la rama [branch]

* git push --force  # Ignorar los cambios locales y hacer push

* git push --all # Subir al repositorio todas las ramas

* git fetch # Traer los commits del repositorio remoto al repositorio local

#### 4.- Ramas
* git branch [branch-name]  # Crear una rama desde la rama actual

* git branch [branch-name] [initial-branch]  # Crear rama a partir de otra rama

* git branch -m [branch-name]  # Cambiar de nombre a la rama actual

* git branch -m [branch-name] [new-branch-name]  # Cambiar de nombre una rama

* git branch -d [branch-name]  # Eliminar una rama

* git checkout [branch-name]  # Moverse a una rama concreta

* git checkout -b [branch-name]  # Crear una rama y moverse a esa rama

* git merge [branch-name]  # Unir la rama actual con la rama seleccionada

* git merge [branch-name] [initial-branch]  # Unir una rama con otra

* git branch -av  # Visualizar las ramas

#### 5.- Etiquetas

* git tag -a [tag-name] -m “Message” # Crear una etiqueta

* git tag # Mostrar las etiquetas

* git show [tag-name] # Mostrar características de una etiqueta en concreto

* git push --tags # Subir las etiquetas al repositorio remoto