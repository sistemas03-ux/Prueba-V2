Git config –global: para realizar una configuración global o no por proyecto.
Git config –global code.editor “code --wait”: Le hacemos entender a git que no esto editor será Visual Studo Code
Git config –global -e: verificamos nuestro archivo de configuración, mantiene la terminal activa hasta que cerremos el editor 
Git init: creación del repositorio de git
Ls -a: no sayuda a mostrar todos lo documentos ocultos.
Git congif nome.user “nombre del usuario”: Asignacion de nombre al usuario que es el mismo que se creo en el inicio de sesión de GitHub 
Git status: nos ayuda a verificar que modificaciones sea han hecho y no se han subido aun.
Git add “nombre del archivo”: nos ayuda a subir o agregar un nuevo archivo al repositorio de manera provisional, seleccionar los archivos para pasarlos a una etapa llamada STAGE para verificar los cambios que hemos hecho y posteriormente pasan al repositorio.
•	Git add  . : sube todos los archivos
•	Git *.txt: agrega todos los archivos con la extensión escrita.
Git commit -m “Nombre del Commit”: Sirve para agregar un archivo de forma permanente, los cambios que nosotros hayamos comprometido y mandarlos a un servidor.
Code .: nos abre la carpeta en donde nos encontramos dentro de nuestro Visual o entorno de desarrollo.
Rm: Sirve para eliminar un archivo.
Git rm NombreDelArchivo: borra completamente el archivo seleccionado y lo deja en la etapa de stage para posteriormente realizar el commit de esa eliminación.
git restore --staged nombredelarchivo: elimina un archivo del área de preparación de Git.
Git restore NombreDelArchivo: Restaura el archivo antes de realizar un commit 
Mv NombreDelArichoActual NuevoNombreDelArhivo:  Nos ayuda a cambiar de nombre a cualquier archivo.
Git mv NombreDelArchivo NuevoNombre: es una manera mas fácil de cambiar el nombre a los archivo y mandarlos a la etapa de STAGE sin hacer dos líneas de comandos.
Git status -s: nos muestras de una manera mas limpia los archivos que se encuentran en stage
Git diff: Nos muestra los cambios que se hacen dentro del archivo.
Git log –oneline: Nos muestra el historial de commits realizados. 
Git push -u *nombre del repositorio “nombre de la rama”: nos ayuda a subir los archivos a nuestro repositorio remoto de GitHub.
Git Branch: nos muestra en que rama estamos trabajando.
Git checkout -b NombreDeLaRama: Nos ayuda a crea una rama y pasarnos a ella.
Git checkout NombreDeLaRama: No ayuda a movernos de rama.
Get merge NombreDeLaRama: sube los archivos de las demás ramas en la rama que se esta
Git push -u *nombre del repositorio “nombre de la rama”: nos ayuda a subir los archivos a nuestro repositorio remoto de GitHub. 
git remote add origin https://github.com/sistemas03-ux/Prueba-V1.git: Para subir nuestro repositorio remoto a github.
