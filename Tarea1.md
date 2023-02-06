# Investigación 1 - Jorge Yxcot 

## 1. Qué es git
------

Se puede definir como un sistema de administración y control de versiones de código distribuido, el cual permite guardar y optimizar diferentes versiones de un mismo proyecto a lo largo del tiempo, se puede trabajar en diferentes cambios, comentar y revisar estos mismos, con la finalidad de probar las diferentes optimizaciones, en caso que se encuentre un problema con estos, se pueden revertir "retrocediendo" a la version anterior sin estos cambios.

Con Git, se puede guardar la información o código generado con cambios (conocido como un "commit") en el repositorio, además de poder trabajar en ramas (branches) separadas del código principal, lo que nos permite experimentar sin afectar el código principal. Lo cual, nos permite, cuando estemos listos y seguros del código a integrar, "fusionar" estos cambios a la rama principal ("master").

![Proceso idoneo de un branch](https://user-images.githubusercontent.com/124539205/216861094-c65a6957-60c8-4f95-b01d-08e717066fa8.png)

El hecho de ser "Distribuido" indica, que al compartir el directorio de un proyecto, Git no sólo comparte la última versión del archivo, sino cada versión que se ha registrado para ese proyecto, brindando mayor contexto sobre el proyecto.


## 2. Qué es github
------

GitHub es una plataforma en línea (al igual que: GitLab, Bitbucket, SourceForge, Cloud Source Repositories, AWS CodeCommit, Azure DevOps) la cual permite el alojamiento y edición de proyectos de software que utilizan el sistema de control de versiones Git. Éste permite tener diferentes ramas del mismo proyecto en diferentes estados según su ciclo de vida dentro del proyecto desarrollado.

Link de referencia útil: [Glosario de Git y Github](https://docs.github.com/es/get-started/quickstart/github-glossary)

## 3. Markdown
------

### Estilo:

**Texto en negrilla debe ir entre dos (2) asteriscos en cada lado**	

*El texto en cursiva va entre un (1) asterisco de cada lado*

~~Este texto está entre dos (2) virgulillas~~ > Este texto está entre dos (2) virgulillas

Para colocar formato a un título, colocamos el simbolo de numeral (#) al inicio de la línea para aplicarlo.
# Título 1

## Título 2

## ...

###### Título 6

### Tablas:

Los tabuladores pueden ser utilizados para formatear columnas de una tabla.

Prueba | de | Tabla
--- | --- | ---
*Simple* | `pero` | **entendible**
A | B | C


Debe haber al menos 3 guiones separando cada encabezado.
Los pipes exteriores (|) son opcionales y no son necesarios para que github lo entienda.

### Código en Github:
Para formatear código o texto en su propio bloque distintivo, usa comillas triples.

```
git status
git add
git commit
```

### Listas
Para crear listas ordenadas basta con escribir los elementos enumerados al inicio de cada línea (ejemplo aplicado), para crear listas sin ordenar, basta con escribir los elementos con asteriscos, guiones o signo más (-, * o +) antes de las líneas de texto.

* Ejemplo
* de
* una
* lista
* sin
* ordenar

Para crear una lista de tareas, debemos escribir un guión y espacio, seguido de corchetes ([ ]) a los elementos de la lista. Para marcar una tarea como completada, usamos la letra equis entre los corchetes ([x]).

- [x] Tarea realizada
- [ ] Tarea por realizar
- [ ] Tarea 2 por realizar


Link de referencia útil: [Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

## 3.1 Comandos
------
Entre los [comandos más utilizados](https://training.github.com/downloads/es_ES/github-git-cheat-sheet.pdf) en github tenemos:

|Nombre|código|Qué hace|
|---|---|---|
|Git Status|`git status`|Podemos obtener información cómo: Si la rama actual está actualizada, si hay algo que necesita un commit, un add, o borrarse, archivos preparados, sin preparar o sin seguimiento, archivos creados, modificados o eliminados|
|Git clone|`git clone https://name-of-the-repository-link`|Git clone básicamente hace una copia idéntica de la última versión de un proyecto en un repositorio y la guarda en su computadora.|
|Git branch|`git branch <nombre-de-la-rama>`|Creando una nueva rama|
|Git push|`git push -u <remote> <nombre-de-la-rama>`|Se utiliza para insertar la nueva rama en el repositorio remoto|
|Git branch list|`git branch or git branch --list`|Se utiliza para ver las ramas|
|Git Delete Branch|`git branch -d <nombre-de-la-rama>`|Se utiliza para borrar las ramas|
|Git Checkout|`git checkout <nombre-de-la-rama>`|Usamos git checkout principalmente para cambiar de una rama a otra.|
|Git add|`git add <file>` para un solo archivo o bien `git add -A`|Utilizamos el comando git add para incluir los cambios de un archivo en nuestro próximo commit.|
|Git Commit|`git commit -m "commit message"`|Nos permite agregar comentarios y guardar localmente los cambios realizados, como un punto de guardado al que podemos volver.|
|GitPush|`git push <remote> <nombre-de-la-rama>`|Después de confirmar los cambios, con git push podemos subir las confirmaciones al repositorio remoto|
|Git Pull|`git pull <remote>`|Este comando nos permite traer las actualizaciones del repositorio remoto al local|
|Git Revert|`git revert #codigo hash`|Esto nos permite revertir cualquier cambio de commit que hayamos realizado y volvemos a un "punto seguro"|
|Git Merge|`git merge <nombre-de-la-rama>`|El paso final es fusionar la rama en la que trabajamos con la rama principal, para esto siempre se recomienda que la versión sea la misma o la más actualizada para evitar problemas de versionado o funciones.|
