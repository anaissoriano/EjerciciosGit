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

**Ejercicios de repositorios remotos**

Para hacer estos ejercicios es necesario haber hecho antes los ejercicios sobre ramas.

Ejercicio 1
1. Crear un nuevo repositorio público en GitHub con el nombre libro-git.


2. Añadirlo al repositorio local del libro.
~~~
git remote add github https://github.com/anaissoriano/libro-git.git
~~~
3. Mostrar todos los repositorios remotos configurados.
~~~
git remote -v
~~~

Ejercicio 2
1. Añadir los cambios del repositorio local al repositorio remoto de GitHub.

~~~
git push -u github master
~~~

2. Acceder a GitHub y comprobar que se han subido los cambios mostrando el historial de versiones.

~~~
git push https://github.com/anaissoriano/libro-git.git master
~~~

Ejercicio 3
1. Colaborar en el repositorio remoto libro-git de otro usuario.

~~~

~~~

2. Clonar su repositorio libro-git.

~~~
git clone https://github.com/4tomyc/EjerciciosGit.git
~~~

3. Añadir el fichero autores.txt que contenga el nombre del usuario y su correo electrónico.

~~~
notepad autores.txt
~~~

4. Añadir los cambios a la zona de intercambio temporal.

~~~
git add .
~~~

5. Hacer un commit con el mensaje “Añadido autor.”

~~~
git commit -m "Añadido autor."
~~~

6. Subir los cambios al repositorio remoto.

~~~
git push -u github master
~~~

Ejercicio 4

1. Desde vuestra cuenta de GitHub, realizad un «Fork» del repositorio
https://github.com/mcuevaseljust/guiaApunts.git.

~~~

~~~

2. Modificad el fichero README.md, añadiendo vuestro nombre en la tabla.

~~~

~~~

3. Haced un «Pull request» para contribuir en el repositorio de «mcuevaseljust», podéis dejar un comentario.

~~~

~~~

Nota: En este ejercicio, deberéis enviar capturas de los pasos que vayáis llevando a cabo.

Ejercicio 5

1. Clonar el repositorio mcuevaseljust/EjerciciosGit
~~~
git clone https://github.com/mcuevaseljust/EjerciciosGit.git
~~~
2. Crea un repositorio en tu cuenta de GitHub, y sube el repositorio clonado con las soluciones de los diferentes ejercicios.
~~~

~~~
3. Modifica el fichero README.md, indicando tu nombre e indica la dirección del repositorio.
~~~

~~~
