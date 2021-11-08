---   
title: Activitat práctica 3 GIT
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

Ejercicios de deshacer cambios
Para hacer estos ejercicios es necesario haber hecho antes los ejercicios sobre historial de
cambios.


## Ejercicio 1:

1. Eliminar la última línea del fichero indice.txt y guardarlo.

~~~
- nano indice.txt
- Eliminar la ultima linea.
~~~

2. Comprobar el estado del repositorio.

~~~
- git status
~~~

3. Deshacer los cambios realizados en el fichero indice.txt para volver a la versión
anterior del fichero.

~~~
-git checkout indice.txt
~~~

4. Volver a comprobar el estado del repositorio.

~~~
- git status
~~~

## Ejercicio 2:

1. Eliminar la última línea del fichero indice.txt y guardarlo.

~~~
- nano indice.txt
- Eliminar la ultima linea.
- git status
~~~

2. Añadir los cambios a la zona de intercambio temporal.

~~~
- git add .
~~~

3. Comprobar de nuevo el estado del repositorio.

~~~
- git status
~~~

4. Quitar los cambios de la zona de intercambio temporal, pero mantenerlos en el
directorio de trabajo.

~~~
- git restore --staged index.txt
- git reset index.txt
~~~

5. Comprobar de nuevo el estado del repositorio.

~~~
- git status
~~~

6. Deshacer los cambios realizados en el fichero indice.txt para volver a la versión
anterior del fichero.

~~~
- git checkout --indice.txt
~~~

7. Volver a comprobar el estado del repositorio.

~~~
- git status
~~~

## Ejercicio 3:

1. Eliminar la última línea del fichero indice.txt y guardarlo.

~~~
- nano indice.txt
- eliminar la ultima linea
- git status
~~~

2. Eliminar el fichero capitulos/capitulo3.txt.

~~~
- rm capitulos/capitulo3.txt
~~~

3. Añadir un fichero nuevo capitulos/capitulo4.txt vacío.

~~~
- nano capitulos/capitulo4.txt
- git status
~~~

4. Añadir los cambios a la zona de intercambio temporal.

~~~
- git add .
~~~

5. Comprobar de nuevo el estado del repositorio.

~~~
- git status
~~~

6. Quitar los cambios de la zona de intercambio temporal, pero mantenerlos en el
directorio de trabajo.

~~~
- git reset .
~~~

7. Comprobar de nuevo el estado del repositorio.

~~~
- git status
~~~

8. Deshacer los cambios realizados para volver a la versión del repositorio.

~~~
- git checkout -- .
~~~

9. Volver a comprobar el estado del repositorio.

~~~
- git status
~~~

## Ejercicio 4: 

1. Eliminar la última línea del fichero indice.txt y guardarlo.

~~~
- nano indice.txt
~~~

2. Eliminar el fichero capitulos/capitulo3.txt.

~~~
- rm capitulos/capitulo3.txt
~~~

3. Añadir los cambios a la zona de intercambio temporal y hacer un commit con el
mensaje “Borrado accidental.”

~~~
- git commit -m "Borrado accidental"
- git log --oneline
~~~

4. Comprobar el historial del repositorio.

~~~
- git status
~~~

5. Deshacer el último commit pero mantener los cambios anteriores en el directorio de
trabajo y la zona de intercambio temporal.

~~~
- git reset --soft HEAD-1
- git log --oneline
~~~

6. Comprobar el historial y el estado del repositorio.

~~~
- git status
~~~

7. Volver a hacer el commit con el mismo mensaje de antes.

~~~
- git commit -m "Borrado accidental"
- git log --oneline
~~~

8. Deshacer el último commit y los cambios anteriores del directorio de trabajo volviendo
a la versión anterior del repositorio.

~~~
- git reset --hard HEAD-1
- git log --oneline
~~~

9. Comprobar de nuevo el historial y el estado del repositorio.

~~~
- git status
~~~
