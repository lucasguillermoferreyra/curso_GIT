# Clase 05

## GIT RESET

### GIT Reset soft
Elimina los commits que seleccioné pero la info se guarda en el staging area. O index

    git reset --soft <hash>

### GIT Reset mixed
Elimina los commits que seleccioné pero la info se guarda en el working directory.

    git reset <hash>
    git reset --mixed <hash>

### GIT Reset hard (Peligroso)
Por que pierdo lo que tenía dentro de los commits. Es destructivo

    git reset --hard <hash>

## Trabajar en proyectos Open Source (Pull Request)

1. Hacer un fork del proyecto. Del proyecto del cual quiero contribuir (Me copiar en mi cuenta el repo del proyecto original)
2. Me clono el fork desde mi cuenta github
3. Trabajo normalmente. Subo los cambios (A repo propio)
4. Me voy al proyecto original en el apartado Pull Request. Creo un nuevo Pull Request. Algunas veces aparece en mi repo la posibilidad Pull Request.
---
5. Si el repo original sufrió más modificaciones. (Commits). Voy a tener que actualizar mi fork.
6. Voy a la cuenta del proyecto original y me copio la url del repositorio
7. Y agrego en mi repositorio local, la url (el remoto) del proyecto original.

    git remote upstream <URL-repositorio-original>

8. Me traigo los cambios del repositorio original a mi repo local

    git pull upstream <rama-que-quiero-actualizar>

9. Subo a mi repositorio remoto (Fork) las actualizaciones del repo local

    git push origin <rama-a-actualizar>

## Apuntadores

> Apuntadores dinamicos

* HEAD

> Apuntadores estaticos

* RAMAS (Locales y remotas)
* TAG
* STASH
## TAGs

> Listar tags

    git tag

> Crear tags

    git tag <nombre-tag>
    git tag hasta-aca-todo-ok

> Borrar tags

    git tag -d <nombre-tag>
    git tag -d hasta-aca-todo-ok

> Crear tag con versionado semantico

    git tag -a v1.0.0 <hash> -m "Versión 1.0.0"
    git tag -a v1.0.0 f473780 -m "Versión 1.0.0"

* a: anotado
* m: mensaje

> Ver detalle de los tags, quien creo y en que commit están creados

    git show v1.0.0

> Para subir tags especifico (Recomendada)

    git push origin <nombre-tag>
    git push origin v1.0.0

> Para subir todos tags (NO RECOMENDADO)

    git push --tags









