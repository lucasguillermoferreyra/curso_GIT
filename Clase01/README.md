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
> Me muestra las fotos en una linea 
  git log --oneline


# Clase 01

## COMANDO DE CONSOLA BÁSICOS

* ls : Listar directorios
* cd : Cambiar de directorio
    
    cd <directorio>
    cd clase-01

* cd .. : Salgo de un directorio
* touch : Creo archivos vacios

    touch <nombre-archivo>
    touch archivo1.txt archivos2.txt

* mkdir : Creo directorios

    mkdir <nombre-directorio>
    mkdir dir1 dir2 dir3

* rm: Borrar archivos

    rm <archivo-a-borrar>
    rm index.html

* rmdir : Borro directorio 

    rmdir <directorio-a-borrar>
    rmdir dir1

* clear : Limpio la consola

## GIT INTRODUCCIÓN

> Saber si tengo git instalado

    git --version

> Configuración importante de git
GLOBAL: Para todos los repositorios que se creen en el equipo

    git config --global user.name "nombre"
    git config --global user.email "correo"

> Inicializar repositorio git (Crear un repositorio)

    git init

> Configuración de repositorio con un usuario y mail diferente
LOCAL: Configura usuario y mail para el repositorio actual

    git config --local user.name "nombre"
    git config --local user.email "correo"

### GIT STATUS
> Me permite ver los cambios que tengo el Working Directory (WD) respecto del Repositorio

    git status

### GIT ADD
> Me permite agregar archivos al temporal de confirmación de cambio. Siempre tengo que hacer esto cada vez que quiero sacar una foto (commit) 
> Mueve los archivos del WD al Staging Area (Index)

    git add .

### GIT COMMIT
> Sacar la foto, colocar lo que tenía en el Staging area en el repositorio.

    git commit -m "Mensaje"

### GIT LOG
> Me muestra las fotos o los commits que tengo en el repositorio

    git log
    git log --oneline

