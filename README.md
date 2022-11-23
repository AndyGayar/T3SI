
Tarea 3 Andrés Gayar Romero
____

Para posicionarse en el directorio padre del de inicio:
~~~
cd /home
~~~
___
Visualizar ruta directorio actual
~~~
pwd
~~~
Comprobamos el resultado
~~~
andres@andres-VirtualBox:/home$ pwd
/home
~~~
___
 Obtén un listado de todos los ficheros/directorios que cuelgan de tu directorio de
trabajo actual
~~~
ls -la
~~~
Obtenemos:
~~~
total 12

drwxr-xr-x  3 root   root   4096 oct 28 10:20 .

drwxr-xr-x 20 root   root   4096 oct 28 10:17 ..

drwxr-x--- 18 andres andres 4096 nov 21 14:22 andres
~~~
___
Realiza un listado recursivo de tu directorio de inicio.
~~~
 ls -R
~~~
Obtenemos:
~~~
.:

andres



./andres:

1  Descargas   ejercicio   Imágenes  paca        Público  Vídeos

2  Documentos  Escritorio  Música    Plantillas  snap



./andres/1:

basura  clase  grupo



./andres/1/basura:



./andres/2:



./andres/Descargas:



./andres/Documentos:



./andres/Escritorio:



./andres/Imágenes:



./andres/Música:



./andres/Plantillas:



./andres/Público:



./andres/snap:

firefox  snapd-desktop-integration



./andres/snap/firefox:

2067  2088  common  current



./andres/snap/firefox/2067:



./andres/snap/firefox/2088:



./andres/snap/firefox/common:



./andres/snap/snapd-desktop-integration:

14  common  current



./andres/snap/snapd-desktop-integration/14:



./andres/snap/snapd-desktop-integration/common:



./andres/Vídeos:


~~~
___
 Obtén la ayuda del comando passwd.
~~~
 passwd -h
~~~
Obtenemos:
~~~
Modo de uso: passwd [opciones] [USUARIO]



Opciones:

  -a, --all                     informa del estado de las contraseñas de

                                todas las cuentas

  -d, --delete                  borra la contraseña para la cuenta indicada

  -e, --expire                  fuerza a que la contraseña de la cuenta

                                caduque

  -h, --help                    muestra este mensaje de ayuda y termina

  -k, --keep-tokens             cambia la contraseña sólo si ha caducado

  -i, --inactive INACTIVO       establece la contraseña inactiva después de

                                caducar a INACTIVO

  -l, --lock                    bloquea la contraseña de la cuenta indicada

  -n, --mindays DÍAS_MIN        establece el número mínimo de días antes

                                de que se cambie la contraseña a DÍAS_MIN

  -q, --quiet                   modo silencioso

  -r, --repository REP          cambia la contraseña en el repositorio REP

  -R, --root CHROOT_DIR         directorio en el que hacer chroot

  -S, --status                  informa del estado de la contraseña la cuenta

                                indicada

  -u, --unlock                  desbloquea la contraseña de la cuenta indicada

  -w, --warndays DÍAS_AVISO     establece el aviso de caducidad a DÍAS_AVISO

  -x, --maxdays DÍAS_MAX        establece el número máximo de días antes de

                                cambiar la contraseña a DÍAS_MAX


~~~
___
Obtén la fecha y la hora del sistema.
~~~
date
~~~
Obtenemos:
~~~
lun 21 nov 2022 14:10:54 CET
~~~
___
Usando un solo comando posiciónate en tu directorio de inicio
~~~
cd
~~~
Comprobamos:
~~~
andres@andres-VirtualBox:~$ pwd
/home/andres
~~~
___
Crea un fichero materias que contenga el nombre de las materias en las que te has
matriculado (cada una en una línea distinta).

~~~
cat>>materias
Sistemas informáticos
Programación
Bases de Datos
Entornos de Desarrollo
Lenguaje de marcas
FOL
~~~
Usando el comando cat>> creamos un fichero con los datos que introducimos a continuación si no es muy extenso.
___
Con un solo comando, crea dos directorios grado y lru
~~~
mkdir grado Iru
~~~
Comprobamos:
~~~
andres@andres-VirtualBox:~$ ls

1  Descargas   ejercicio   grado     Iru     paca        Público  Vídeos
2 Documentos  Escritorio  Imágenes  Música  Plantillas  snap
~~~
Podemos observar que los directorios han sido creados.
___
Usando un solo comando, mueve tu fichero materias para que cuelgue de tu
directorio grado pero con el nombre asignaturas
~~~
mv materias grado/asignaturas
~~~
Comprobamos:
~~~
andres@andres-VirtualBox:~$ ls grado/
asignaturas

andres@andres-VirtualBox:~/grado$ cat asignaturas
Programación
Sistemas informáticos
Entornos de Desarrollo
Lenguaje de Marcas
Bases de Datos
FOL
~~~
Observamos que se ha creado el fichero asignaturas en grado
___
Visualiza los ficheros/directorios de tu directorio de trabajo actual y responde a la
siguiente cuestión: ¿dónde está tu fichero materias?
~~~
 ls -la 
~~~
No existe ppr que ahora se llama asignaturas y está en grado
___
Posiciónate en tu directorio grado.
~~~
cd grado
~~~
Comprobamos:
~~~
andres@andres-VirtualBox:~/grado$ pwd
/home/andres/grado
~~~
___
Elimina el fichero asignaturas.

~~~
rm asignaturas
~~~
Comprobamos:
~~~
andres@andres-VirtualBox:~/grado$ ls
andres@andres-VirtualBox:~/grado$ 
~~~
No muestra nada porque está vacio al quitar asignaturas, que era el único fichero
___
Sube al directorio de inicio.

~~~
cd
~~~
Comprobamos:
~~~
andres@andres-VirtualBox:~$ pwd
/home/andres
~~~
___
Con un solo comando elimina los directorios creados en el paso i)
~~~
rmdir grado Iru
~~~
Comprobamos:
~~~
andres@andres-VirtualBox:~$ ls

1  Descargas   ejercicio   Imágenes  paca        Público  Vídeos
2  Documentos  Escritorio  Música    Plantillas  snap
~~~
No existen Iru ni grado por lo que hemos acabado el ejercicio
