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

