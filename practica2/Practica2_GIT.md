---   
title: Activitat práctica 2 GIT
titlepage: true
titlepage-rule-height: 0
titlepage-rule-color: 653097
toc-own-page: true
toc-title: Contenidos
header-left: EDD
header-right: Activitat GIT
lang: es-ES
footer-left: IES Jaume II el Just
footer-right: \thepage/\pageref{LastPage}
titlepage-background: git.png

---

# Act practica GIT:

**Creación y actualización de repositorios.**

## Ejercicio 1:
1. Mostrar el historial de cambios del repositorio.
~~~
git log
git log --oneline
~~~
2. Crear la carpeta capitulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto:"Git es un sistema de control de versiones ideado por Linus Torvalds."
~~~
mkdir capitulos
ls -la
vim capitulos/capitulo1.txt "Git es un sistema de control de versiones ideado por Linus Torvalds."
ls -la
~~~
3. Git es un sistema de control de versiones ideado por Linus Torvalds.

4. Añadir los cambios a la zona de intercambio temporal.
~~~
git add .
git status
~~~
5. Hacer un commit de los cambios con el mensaje “Añadido capítulo 1.”
~~~
git config --global.user.name Anais
git config --global user.email anaisclase13@gmail.com
git commit -m "Añadido capitulo 1."
~~~
6. Volver a mostrar el historial de cambios del repositorio.
~~~
git log
git log --oneline
~~~

## Ejercicio 2:

1. Crear el fichero capitulo2.txt en la carpeta capitulos con el siguiente texto.

~~~
-vim capitulos/capitulo2.txt 
-"El flujo de trabajo básico con Git consiste en: 1- Hacer cambios en el repositorio.
~~~

2. Añadir los cambios a la zona de intercambio temporal.

~~~
-git add .
-git status
~~~

3. Hacer un commit de los cambios con el mensaje “Añadido capítulo 2.”

~~~
-git commit -m "Añadido capitulo 2."
-git log --oneline
~~~

4. Mostrar las diferencias entre la última versión y dos versiones anteriores.

~~~
-git diff HEAD~2..HEAD
-git log
~~~

## Ejercicio 3:

1. Crear el fichero capitulo3.txt en la carpeta capitulos con el siguiente texto.

~~~
-vim capitulos/capitulo3.txt "Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas."
-git status
~~~

2. Añadir los cambios a la zona de intercambio temporal.

~~~
-git add .
-git status
~~~

3. Hacer un commit de los cambios con el mensaje “Añadido capítulo 3.”

~~~
-git commit -m "Añadido capitulo 3."
~~~

4. Mostrar las diferencias entre la primera y la última versión del repositorio.

~~~
-git diff HEAD~1..HEAD
-git log
~~~

## Ejercicio 4:

1. Añadir al final del fichero indice.txt la siguiente línea:

~~~
-vim indice.txt
añadir: "Capitulo 5: Conceptos avanzados."
~~~

2. Añadir los cambios a la zona de intercambio temporal.

~~~
-git add .
-git diff
~~~

3. Hacer un commit de los cambios con el mensaje “Añadido capítulo 5 al índice.”

~~~
-git commit -m "Añadido capitulo 5 al indice."
~~~

4. Mostrar quién ha hecho cambios sobre el fichero indice.txt.

~~~
-git annotate indice.txt
~~~
