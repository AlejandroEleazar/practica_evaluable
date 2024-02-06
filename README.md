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

