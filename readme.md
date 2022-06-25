# Git Desarrollo Colaborativo

Esto es una guia creada con la finalidad de facilitar el entendimiento y aplicacion de la herramienta conocida como GIT, que se utiliza para el control de versiones de nuestros proyectos. Aqui veremos como configurar la misma, asi como tambien, cada una de sus opciones.

## Configuracion Inicial

Cuando inicializamos un repositorio por primera vez, podemos establecer el nombre de usuario y correo electronico, para identificarnos dentro del historial de cambios. 

Cuando queremos definir una configuracion de manera Gral, debemos utilizar __--global__ para indicar que dicha configuracion debe almacenarse en la carpeta del usuario y no en la carpeta __.git__ del repositorio.

* __git init__: Inicializa un repositorio de GIT.
* __git config --global user.name__ `username`: Define el nombre de usuario para el control de cambios.
* __git config --global user.email__ `email`: Establece el correo electronico para las confirmaciones.

## Gestion del Proyecto

para sincronizar los cambios realizados en el proyecto, debemos tener en cuenta que si creamos en nuestra compu el mismo utilizando el comando __git init__, vamos a tener que crearlo tambien en nuestro servidor remoto, como por ejemplo [Github](https://github.com). 

En caso que ya exista un repositorio remoto, simplemente debemos descargar el historial de cambios del mismo, pero indistintamente de como hayamos empezado, lo principal es estar pendiente de los cambios realizados en el servidor de GIT.