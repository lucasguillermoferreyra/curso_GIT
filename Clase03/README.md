### GIT RANAS
> Para crear rama 
   git branch <nombre de la rama>

> Para cambiar de rama
  git switch <nombre de la rama> 

> Para borrar rama 
  git branch -d <nombre de la rama>

> Para forzar el borrado sin hacer un marge (no la pegue a ninguna rama)
  git branch -D <nombre de la rama>

### GIT MARGE
>Para fusionar ramas
  git marge <nombre de la rama>


# Clase 03
## GIT RAMAS (Branchs) - REPASO

> Crear una rama

    git branch <nombre-rama>
    git branch dev

> Moverme entre ramas

    git switch <nombre-rama>
    git switch dev

> Para ver las ramas

    git branch

> Para borrar una ramas

    git branch -d <nombre-rama>
    git branch -d dev

> Para forzar el borrado de una ramas
Recuerden que este flag me sirve para confirmar el borrado de una rama que no fue fusionada con ninguna otra.

    git branch -D <nombre-rama>
    git branch -D dev

## GIT MERGE (Funsiones)
Combinar los cambios de una rama con otra. Normalemnte en un nuevo commit
**IMPORTANTE:** Tengo que estar en la rama que espero traerme los cambios. O sea si quiero traerme los cambios de dev a master tengo que estar sobre la rama master y ejecutar el siguiente comando

    git merge <nombre-rama>
    git merge dev

### Abortar la funsión (El merge)

    git merge --abort

### Tipos de Fusiones/Merge

* Fast-forward (Unión automática) Git no necesita de la asistencia del usuario. Tampoco hay conflictos

* Recursivo (Unión automática). Tampoco hay conflictos.

* Manual (Conflictos) Ocurre cuando hay modificaciones en las mismas líneas de un archivos o varios archivos.