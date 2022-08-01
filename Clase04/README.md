# Clase 04

## GIT CHERRY PICK

**IMPORTANTE:** Tengo que estar ubicado en la rama que espero traerme el o los commits.

    git cherry-pick <hash>
    git cherry-pick <hash1> <hash2> <hash3>

```sh
    git cherry-pick <hash>^..<hash> #Todos los commits incluidos en el rango y además los extremos
```
```sh
    git cherry-pick <hash>..<hash> #Solo me trae los que están entre esos 2 commits, no las puntas
```

### SI tengo varios commits, no uno. Voy a tener que hacer

    git cherry-pick --continue

### Para abortar el proceso de cherry-picking

    git cherry-pick --abort

## GIT ALIAS

### Para crear alias

    git config --global alias.ll "log --oneline --decorate --all --graph"
    git config --global alias.l "log --oneline"
    git config --global alias.s "status --short"
## Para listar alias

    git config --get-regexp alias

## Para quitar un alias

    git config --global --unset alias.s


## GIT STASH
Es construido basado en una estructura de datos conocida como pila.

> ¿Qué me permite el stash?

Me permite registrar temporalmente los cambios del Working Directory y el Staging AREA.

> ¿Puedo subir al remoto los stash?

No. Solo están en el repositorio local. No se pueden subir al remoto.

### Crear un stash

    git stash

### Listar los stash

    git stash list

### Recuperar un stash

**Nota:** Si el stash que estoy tratando de recuperar genera un conflico con mi código, o sea con el código que esta en el repositorio. Me va a dejar en la caja el stash que estoy sacando. Si no hay conflictos, borra el stash.

    git stash pop

### Borrar el último stash

    git stash drop
    git stash drop stash@{4}


### Si quiero aplicar un stash particular (Solo aplica, no borra lo aplicado)

    git stash apply stash@{4}
    git stash apply stash@{2}

### Si quiero aplicar un stash en una rama nueva.

    git stash branch <rama-a-aplicar-stash>


## Versiones DESKTOP

* Git Kraken: https://www.gitkraken.com/
* Github Desktop: https://desktop.github.com/

## Buenas prácticas para generar mensajes de commits

https://medium.com/@jmz12/buenas-pr%C3%A1cticas-para-commits-5eb4c86b9a47
