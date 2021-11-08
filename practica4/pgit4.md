---   
title: Activitat práctica 4 GIT
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

**Ejercicios de gestión de ramas.**


Para hacer estos ejercicios es necesario haber hecho antes los ejercicios sobre historial de
cambios.


Ejercicio 1

Crear una nueva rama bibliografia y mostrar las ramas del repositorio.

~~~
git branch bibliografia
~~~

Ejercicio 2

1. Crear el fichero capitulos/capitulo4.txt y añadir el texto siguiente
~~~
vim capitulos/capitulo4.txt
~~~

2. Añadir los cambios a la zona de intercambio temporal.
~~~
git status
~~~
3. Hacer un commit con el mensaje “Añadido capítulo 4.”
~~~
git commit -m "Añadir capitulo 4."
~~~
4. Mostrar la historia del repositorio incluyendo todas las ramas.
~~~
git log --graph --all --oneline
~~~

Ejercicio 3

1. Cambiar a la rama bibliografia.
~~~
git checkout bibliografia
~~~

2. Crear el fichero bibliografia.txt y añadir la siguiente referencia

~~~
  vim bibliografia.txt
"·Chacon 5, and Straub, B, Pro Git, Apress."
~~~

3. Añadir los cambios a la zona de intercambio temporal.
~~~
git add .
~~~
4. Hacer un commit con el mensaje “Añadida primera referencia bibliográfica.”
~~~
git commit -m "Añadida primera referencia bibliográfica."
~~~
5. Mostrar la historia del repositorio incluyendo todas las ramas.
~~~
git log --graph --all --oneline
~~~

Ejercicio 4

1. Fusionar la rama bibliografia con la rama master.
~~~
git checkout master
git merge bibliografia
~~~

2. Mostrar la historia del repositorio incluyendo todas las ramas.
~~~
git log --graph --all --oneline
~~~

3. Eliminar la rama bibliografia.
~~~
git branch -d bibliografia
~~~

4. Mostrar de nuevo la historia del repositorio incluyendo todas las ramas.
~~~
git log --graph --all --oneline
~~~

Ejercicio 5

1. Crear la rama bibliografia.
~~~
git branch bibliografia
~~~
2. Cambiar a la rama bibliografia.
~~~
git checkout bibliografia
~~~
3. Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias:
~~~
vim bibliografia.txt
"· Scott Chacon and Ben Straub, Pro Git, Apress.
 ·Ryan Hodson. Ry's Git Tutorial. Smashwords."
~~~
4. Añadir los cambios a la zona de intercambio temporal y hacer un commit con el
mensaje “Añadida nueva referencia bibliográfica.”
~~~
git add .
git commit -m "Añadida nueva referencia bibliográfica."
~~~
5. Cambiar a la rama master.
~~~
git checkout master
~~~
6. Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias:
~~~
vim bibliografía.txt
"·Chacon,S and Straub, B. Pro Git. Apres.
 ·Loelieger, J and McCullough, M.Version control with Git. O'Reilly."
~~~
7. Añadir los cambios a la zona de intercambio temporal y hacer un commit con el
mensaje “Añadida nueva referencia bibliográfica.”
~~~
git add .
git commit -m "Añadida nueva referencia bibliográfica."
~~~
8. Fusionar la rama bibliografia con la rama master.
~~~
git checkout master
git merge bibliografia
~~~
9. Resolver el conflicto dejando el fichero bibliografia.txt con las referencias:
~~~
nano bibliografia.txt
~~~
10. Añadir los cambios a la zona de intercambio temporal y hacer un commit con el
mensaje “Resuelto conflicto de bibliografía.”
~~~
git add .
git commit -m "Resuelto conflictos de bibliografia." 
~~~
11. Mostrar la historia del repositorio incluyendo todas las ramas.
~~~
git log --graph --all --oneline
~~~
