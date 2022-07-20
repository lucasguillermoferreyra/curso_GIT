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