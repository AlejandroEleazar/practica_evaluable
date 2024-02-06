# Comandos de GIT
## Repositorio

>Creacion de un repositorio local

Creacion de un repositorio en GIT

`git init [nombre del repositorio]`

#

>Comprobar el Estado del repositorio

 visualizar los cambios realizados en el working directory y en el área de staging
 
`git status`

#

## Staging

>Añadir ficheros a la carpeta de preparación

 Añadir un fichero especifico al staging
 
`git add [nombre del fichero]`

Añadir un directorio especifico al área de preparación

`git add [directorio]`

Añadir todos los ficheros modificados al staging

`git add .`

#

## Working

>Aprobar los cambios

Validar los cambios realizados

`git commit -m ["mensaje de validación"]`

#

## Versiones

>Revisiones

Ver las revisiones del repositorio

`git log`

Ver las reviciones de forma abreviada

`git log --oneline`

#

>Cambios

Ver los cambios realizados en todos los commits

`git show`

Ver los cambios realizados en un commit en concreto

`git show [idComit]`

#

## Deshaciendo cambios

> Deshacer cambios en el Working

Reemplazar todo lo que haya en el área de working por la última versión valida del HEAD

`git checkout`

Reemplazar todo el contenido del working

`git checkout .`

Deshacer los cambios en un fichero especifico

`git checkout [nombre del fichero]`

#

> Deshacer cambios en el staging

Eliminar el HEAD del staging

`git reset` o `git reset HEAD`

Eliminar un fichero concreto del Staging

`git reset [nombre del ficheor]` o `git reset HEAD [nombre del fichero]`

#

> Deshacer cambios en el staging y en el working

Eliminar los cambios permanentemente no  guardados y restablecer el directorio de trabajo

`git reset --hard`

Eliminar los cambios permanentemente no  guardados y restablecer el directorio de trabajo de un fichero determinado

`git reset --hard [id commit]`

#

> Deshacer cambios del último commit

Deshacer los cambios realizados en el último commit

`git revert HEAD`

#

## Trabajar en remoto

> Repositorio remoto

Vincularse a con un repositorio remoto

`git remote add origin [link repositorio remoto]`

Subir los commits del repositorio local al remoto

`git push`

Ver el repositorio remoto con el que esta vinculado el repositorio local

`git remote -v`

Cambiar el repositorio remoto vinculado

`git remote set-url origin [link repositorio remoto]`

#

> Clonar repositorio remoto

Clonar el repositorio remoto al repositorio local

`git clone [link repositorio remoto] .`

#

## Ramas

> Crear ramas

Crear una nueva rama

`git branch [nombre de la rama]`

#

> Visualizar ramas

Visualizar las ramas del repositorio local

`git branch`

Visualizar las ramas del repositorio local y remoto

`git branch -a`

Visualizar las ramas del repositorio local con el commit del head

`git branch -v`

#

> Cambio de rama

Cambiar de rama

`git checkout [nombre de la rama]`

#

> Renombrar rama

Cambiamor el nombre de una rama

`git branch -m [nuevo nombre]`

#

>Fusionar rama

Fusionar los cambios realizados en las distintas ramas

`git merge [rama origen][rama destino]`

#

>Subir rama al repositorio remoto

Subir rama del repositorio local al repositorio remoto

`git push origin [rama local 1][rama local 2]`

#

>Eliminar rama

Eliminar una rama local

`git branch -d [nombre de la rama]`

#

## Etiquetas

> Crear etiqueta

Crear una etiqueta que se asocie automáticamente al HEAD

`git tag -a [nombre de la etiqueta] -m [mensaje de la etiqueta]`

Crear una etiqueta que se asocir a un commit especifico

`git tag -a [nombre de la etiqueta] -m [mensaje de la etiqueta] [id commit] `

#

> Mostrar etiqueta

Mostrar una etiqueta

`git show [nombre de la etiqueta]`

#

> Eliminar etiqueta

Elimir una etiqueta

`git tag -d [Nombre de la etiqueta]`

#

> Subir etiqueta

Subir una etiqueta especifica del repositorio local al repositorio remoto

`git push origin [nombre de la etiqueta]`

Subir las etiquetas del repositorio local al repositorio remoto

`git push origin --tags`

#
