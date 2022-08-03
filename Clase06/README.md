# Clase 06
Fecha 01/08/2022

## Programas para gestionar los repos

* GitHub Desktop

<https://desktop.github.com/>

* GitKraken

<https://www.gitkraken.com/>

* Sourcetree

<https://www.sourcetreeapp.com/>

* Git Fork

<https://git-fork.com/>

## Repositorios en la nube

* GitHub

<https://github.com/>

* GitLab

<https://about.gitlab.com/>

* Bitbucket

<https://bitbucket.org/>

## Documentación GIT

> Oficial
<https://git-scm.com/book/es/v2>

> Atlassian (Bitbucket)

<https://www.atlassian.com/es/git/tutorials>

## GIT REBASE
Integra los cambios de la rama **master** en una nueva rama **rebase** que le faltan los commits que en **master** están. 

    git rebase <rama-que-me-quiero-traer>
    git rebase master

Una vez solucionados los conflictos con 

    git add

Continuo el rebase con

    git rebase --continue

## GIT ADD (Continuación)

    git add --patch

y: Para confirmar el hunk (Pedacito código)
n: Para descartar el hunk (Pedacito código)

## GIT REBASE INTERACTIVO (AVANZADO)

### ¿Para qué sirve?

* Ordenar commits
* Corregir mensajes de los commits
* Unir Commits
* Separar commits

```sh
    git rebase -i <hash> # Inmediato inferior a lo que quiero seleccionar
```

Una vez seleccionos los commits tengo que seguir los pasos que me diciendo git.

> r, reword: Cambiar el mensaje del commit.
> s, squash: Nos permite funsionar commits. 