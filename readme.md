# Primeros pasos git
> Lista de comandos
~~~
git
~~~
> Crea una carpeta oculta llamada .git en el directorio donde se ejecuta el comando. Esta carpeta contiene todos los archivos necesarios para el repositorio, incluyendo la configuración, historial de compromisos, y o sí archivos que Git utiliza internamente para rastrear los cambios
~~~
git init
~~~
> Establece nombre de usuario
~~~
git config --global user.name "TuNombreDeUsuario"
~~~
> Establece email
~~~
git config --global user.email "TuCorreo@ejemplo.com"
~~~
> Muestra el estado del proyecto
~~~
git status
~~~
> Muestra el listado de archivos en el protecto
~~~
git status -s
~~~
> Mueve los cambios de un archivo al area del entorno de ensayo
~~~
git add NombreArchivo.txt
~~~
> Mueve todos los archivos modificados, nuevos o eliminados al entorno de ensayo
~~~
git add .
~~~
> Es similar a git add ., pero asegura que se incluyan todos los cambios en el proyecto, sin importar el directorio actual
~~~
git add -A
~~~
> Captura la instantanea de los cambios actuales preparados del proyecto
~~~
git commit -m "Escribe un mensaje"
~~~
> Crea un repositorio en la cuenta de GitHub establecida
~~~
curl -u "TuUsuario:TOKEN" https://api.github.com/user/repos -d "{\"name\":\"mi-proyecto-ejemplo\"}"
~~~
> Gestiona las ramas en Git. Mueve (o renombra) la rama actual a un nuevo nombre y, si una rama con ese nombre ya existe, la sobrescribe
~~~
git branch -M nombreRama(main)
~~~
> Se utiliza para conectar tu repositorio local a un repositorio remoto (por ejemplo, en GitHub, GitLab, Bitbucket, etc.). Esto permite que puedas subir y sincronizar los cambios de tu repositorio local con el repositorio en linea
~~~
git remote add origin https://github.com/TuUsuario/TuRepositorio.git
~~~
> Muestra cada confirmacion en una sola línea
~~~
git log --oneline
~~~
> Envia una o mas ramas locales a un repositorio remoto (origen)
~~~
git push origin nombreRama(main)
~~~