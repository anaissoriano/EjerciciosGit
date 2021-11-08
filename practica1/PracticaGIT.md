---   
title: Activitat práctica 1 GIT
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


Ejercici 1 :

1. Crear un repositorio nuevo con el nombre libro y mostrar su contenido
~~~
- mkdir libro
- cd libro
- ls -la
- git init
- ls -la
~~~
2. Configurar Git definiendo el nombre del usuario, el correo electrónico y activar el
coloreado de la salida. Mostrar la configuración final.
~~~
- git config --global.user.name
- git config --global user.email
- git config --list
~~~

Ejercici 2 :

1. Comprobar el estado del repositorio.
~~~
- git status
~~~
2. Crear un fichero indice.txt con el siguiente contenido:
~~~
- vim indice.txt
    - capitulo 1: Introducción a Git 
    - Capitulo 2: Flujo de trabajo basico
    - Capitulo 3: Repositorio remoto
~~~

3. Comprobar de nuevo el estado del repositorio.
~~~
- git status
~~~
4. Añadir el fichero a la zona de intercambio temporal.
~~~
- git add 
~~~
5. Volver a comprobar una vez más el estado del repositorio.
~~~
- git status
~~~

Ejercici 3 :

Realizar un commit de los últimos cambios con el mensaje “Añadido índice del libro.” y ver el estado del repositorio.

~~~
- git commit -m "Añadido indice del libro" 
~~~
~~~
- git log
~~~
~~~
- git show
~~~

Ejercici 4 :

1. Cambiar el fichero indice.txt para que contenga lo siguiente:
~~~
- vim indice.txt
~~~
~~~
    - Capitulo 1: Introducción a Git 
    - Capitulo 2: Flujo de trabajo basico
    - Capitulo 3: Gestión de ramas
    - Capitulo 4: Repositorio remoto
~~~
2. Mostrar los cambios con respecto a la última versión guardada en el repositorio.
~~~
- git diff
~~~
3. Hacer un commit de los cambios con el mensaje “Añadido capítulo 3 sobre gestión de
ramas”
~~~
- git log
~~~
~~~
- git show
~~~

Ejercici 5 :

1. Mostrar los cambios de la última versión del repositorio con respecto a la anterior.

~~~
- git log
~~~

2. Cambiar el mensaje del último commit por “Añadido capítulo 3 sobre gestión de ramas al índice.”

~~~
- git commit --amend -m "Añadido capitulo 3 sobre gestión al indice"
~~~

3. Volver a mostrar los últimos cambios del repositorio.
~~~
- git log
~~~
~~~
- git show
~~~

Ejercici 6 :

Indica a Git que quieres que ignore todos los ficheros que empiecen per “dam”, todos los que
tengan la extensión out y las imágenes (jpg, png, bmp y gif). 

~~~
- vim.gitignore
    - dam* (Todo lo que empiece por dam lo ignora)
    - *.out
    - .jpg
    - .bmp
    - .gif
    - .png
~~~

