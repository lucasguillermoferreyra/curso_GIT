# Clase 01

### COMANDOS DE CONOLA BÁSICOS

* ls: listar directorios 
* cd: Cambiar de directorio 
* cd..: Salgo de un directorio
* touch: creo archivos vacios 
* mkdir: creo directorio
* rm: borra archivos
* rmdir: borra directorios

### GIT Introducción 
> Configuración importante de git
GLobal: para todos los repositorios
git config --globla user.name "Nombre de Usuario"
git config --global user.email "lucasguillermoferreyra@gmail.com"

Local: repositorio actual 
git config --local user.name "Nombre de Usuario"
git config --local user.email "lucasguillermoferreyra@gmail.com"

> para inicializar repositirios en git ejecuto  
 git init

 ### GIT STATUS
  > Me permite ver los cambios que tengo en el Working Directory respecto del repositorio  
   git status

### GIT ADD
 > Me permite agregar archivos al temporal de confoirmación de cambio. Siempre tengo que hacer esto cada vez que quiero sacar una foto (commit)
 > Mueve los archivos del WD a Ataging Area (Index)
   git add.
### GIT COMMIT
 > Sacar la foto, colocar la que tenía en al Staging area en el repositorio 
   git. commit -m "Mensaje"

### GIT LOG
 > Me muestra las fotos o los commits que tengo en el repositorio 

  git log
  git log --oneline