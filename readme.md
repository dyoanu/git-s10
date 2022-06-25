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

### Acceso por primera vez

Cuando clonamos un repositorio remoto debemos tener en cuenta que no exista en la ruta actual ninguna carpeta con el mismo nombre que dicho repositorio, o cualquier nombre que querramos ponerle. Esto se debe a que GIT por cuestiones de seguridad, evitara sobreescribir archivos existentes. Si realizamos esta tarea con exito, se agregara una direccion remota con el nombre __origin__.

* __git clone `romete` `folder`__: Crea una carpeta en donde se descargara el contenido del repositorio.
* __cd `folder`__: Abre la carpeta creada utlizando el comando git clone.

### Sincronizacion de cambios

Una vez clonado un proyecto, debemos tener en cuenta que sus cambios no se sincronizan automaticamente, si no que debemos enviar y descargar los mismos periodicamente; ya que de lo contrario estariamos trabajando en un proyecto que se encuentra desactualizado, y si bien podemos seguir integrando dichos cambios, se dificultaria esta tarea.

* __git fetch `remote`__: Descarga el historial de cambios del repositorio.
* __git pull `remote` `branch`__: Descarga los cambios y los integra a la rama actual.
* __git push `remote` `branch`__: Envia los cambios locales al repositorio remoto.