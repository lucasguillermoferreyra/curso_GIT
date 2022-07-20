## GIT REMOTE 
 git rmeote <url>

## Verificar los reomotos
 git remote 
 git remote -v

## Para subir el repo al remoto
  git push -u origin master

## GITIGNORE
>Me permite descartar archivos y carpetas que no quiero subir al repo remoto 
## GITKEEP
>Me permite mantener y versionar carpetas vacias 

## GIT COMMIT

### Para hacer un commit
>Los archivos que quiero hacer en commit deben estar en seguimiento. Si los archivos no estan en seguimiento (o sea untracked) no los agrega al add

    git commit -m "Mensaje"

### Para hacer un git add y un git commit en simultaneo 

   git add <file>; git commit -m "Mnesaje"

### Para enmendar un commit
   
   git add .
   git commit --amend

 # Clase 02

## GIT REMOTE

### Agregar remoto

    git remote add origin <URL>
    git remote add origin https://github.com/mlapeducacionit/59710-git.git

### Verificar los remotos

    git remote
    git remote -v

### Para subir el repo local al remoto

    git push -u origin master

## GITIGNORE
Me permite descartar archivos y carpetas que no quiero subir.

## GITKEEP
Me permite mantener y versionar carpetas vacías.

## GIT COMMIT

### Para hacer un commit 

    git commit -m "Mensaje"

### Para hacer un git add y un git commit en simultaneo
Los archivos que quiero hacer commit deben estar en seguimiendo. Si los archivos no están en seguimiento (O sea Untraked) no me los va a agregar el git add.

    git commit -am "Mensaje"

### Para enmendar un commit

Agrego los archivos que me olvidé

    git add clase-02/cualquiera.md
Y luego hago el amend

    git commit --amend

## Status de archivos

* Untracked: Archivos que no se agregaron al index (staging area) o sea archivos que están en el Working Directory (WD)

* Unmodified: Son archivos que ya están en el repositorio. O sea ya tienen una foto

* Modified: Son archivos que ya están en el repositorio pero respecto al Working Directory tienen modificaciones detectadas por git. O sea compara la foto del repositorio con el WD.

* Staged: Archivos que están confirmados para ser un próximo commit.

## GIT LOG

### Me muestra una cantidad especifica de commit

    git log --help

> Me muestra los últimos 2 commits
    
    git log -2

> Me muestre los commit por

    git log --since="2022-05-01"
    git log --after="2022-06-01"
    git log --before="2022-05-01"
    git log --after="2022-05-01" --before="2022-05-10"

## GIT RAMAS (Branchs)

> Crear una rama

    git branch <nombre-rama>
    git branch dev

> Moverme entre ramas

    git switch <nombre-rama>
    git switch dev

> Para ver las ramas

    git branch  