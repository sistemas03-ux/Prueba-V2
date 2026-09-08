CONCEPTO TEORICO:
Git Hub sistema de gestión de versiones de software, registra los cambios realizados sobre un archivo o conjunto de archivos a lo largo del tiempo.
Git nos permite a gestionar las distintas versiones de un mismo archivo, pudiendo volver a una versión o una más reciente cuando sea necesario.
Un repositorio done podemos guardas cosas, existen dos tipos de repositorios 
1.	Local: No son compartidos o poniéndolo en red.Git
2.	Remoto: Son lo que se encuentran alejados en algunos servidores externos.
Configuración del entorno de GitHub
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


Administrator@DESKTOP-B35M9DA MINGW64 ~/documents/GiThUB/Practica (master)
$ git log --oneline
25ccac9 (HEAD -> master, origin/master) Conflicto tres corregido
3cd996b Enabezado mejorado
dcefcaa (conflicto-3) Cambio en el acerca
a7fc0c0 Probel resuelto del conflicto 2
0aab53a Actualizacion del input mejorado
5ea8246 (conflicto-2) Actualizacion del input
d7a57ac Primer probelma en el encabezado
7c501de Actualizacion del titulo
2b2be5e (conflicto-1) Actualizacion del titulo
35dc6aa (Rama2) Cracionde archivo html en la carpeta de la rama 2
16aa9eb Cambio de nombre del archivo contacto a contactoCopia
4788ee1 Modificaciones De Contacto desde master
ef71179 Modificacion del index desde la Rama1
dd0d799 Notas agregadas V1
9332306 Agregacion de reglas de archivos ignorados
efa2487 Pie de magina de index
6cd3059 Agrgacion de los estilos de navegacion
b3f2878 Formulario para la pagina de contacto
5f8c25f Pagina de contacto agregada
e9382af Pagina de acerca modificada
271e829 Menu agregado
e21b991 Conexiond de estilos en index
87e7ab2 Estilos declarados
fc34b54 Estructura incial del sitio

Administrator@DESKTOP-B35M9DA MINGW64 ~/documents/GiThUB/Practica (master)
$

Administrator@DESKTOP-B35M9DA MINGW64 ~/documents/GiThUB/Practica (master)
$ git log --graph
*   commit 25ccac932bcd772d790eda32d7a00d8c7a59333f (HEAD -> master, origin/master)
|\  Merge: 3cd996b dcefcaa
| | Author: sisteas03-ux <sistemas03@accounty.mx>
| | Date:   Tue Sep 8 10:58:53 2026 -0600
| |
| |     Conflicto tres corregido
| |
| * commit dcefcaa83a811f07a1c9d7428b66cfa3e0e77700 (conflicto-3)
| | Author: sisteas03-ux <sistemas03@accounty.mx>
| | Date:   Tue Sep 8 10:55:23 2026 -0600
| |
| |     Cambio en el acerca
| |
* | commit 3cd996b9b08876afabad682cb056bcb8db99a8d9
|/  Author: sisteas03-ux <sistemas03@accounty.mx>
|   Date:   Tue Sep 8 10:57:22 2026 -0600
|
|       Enabezado mejorado
|
*   commit a7fc0c02aff8a3db73dac595b5e7c73f1e20c080
|\  Merge: 0aab53a 5ea8246
| | Author: sisteas03-ux <sistemas03@accounty.mx>
| | Date:   Tue Sep 8 10:54:05 2026 -0600
| |
| |     Probel resuelto del conflicto 2
| |

Administrator@DESKTOP-B35M9DA MINGW64 ~/documents/GiThUB/Practica (master)
$

Administrator@DESKTOP-B35M9DA MINGW64 ~/documents/GiThUB/Practica (master)
$ git log --all
commit 25ccac932bcd772d790eda32d7a00d8c7a59333f (HEAD -> master, origin/master)
Merge: 3cd996b dcefcaa
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:58:53 2026 -0600

    Conflicto tres corregido

commit 3cd996b9b08876afabad682cb056bcb8db99a8d9
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:57:22 2026 -0600

    Enabezado mejorado

commit dcefcaa83a811f07a1c9d7428b66cfa3e0e77700 (conflicto-3)
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:55:23 2026 -0600

    Cambio en el acerca

commit a7fc0c02aff8a3db73dac595b5e7c73f1e20c080
Merge: 0aab53a 5ea8246
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:54:05 2026 -0600

    Probel resuelto del conflicto 2

commit 0aab53a8ada1ff87c6474e1ed22c23682c49353d
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:52:42 2026 -0600

    Actualizacion del input mejorado

commit 5ea82463e4eb32e591a8e8a8f76591ed8fe07d41 (conflicto-2)
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:51:55 2026 -0600

    Actualizacion del input

commit d7a57ac3893d7b4132f19021c7898a949710b861
Merge: 7c501de 2b2be5e
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:49:57 2026 -0600

    Primer probelma en el encabezado

commit 7c501dec21a1962bded4ef592b709afc5536b6c5
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:47:59 2026 -0600

    Actualizacion del titulo

commit 2b2be5ed846b0eb712484187309ef32b9ccfc422 (conflicto-1)
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:46:49 2026 -0600

    Actualizacion del titulo

commit 44b5f16b8e271cedd941742a427f97a7d229b85d (Rama1)
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:32:04 2026 -0600

    No se que paso

commit 35dc6aa85cad14451e7dafe73bd4b7bfcb51d34e (Rama2)
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:29:09 2026 -0600

    Cracionde archivo html en la carpeta de la rama 2

commit 16aa9eb997eea7152a32d5c076bb72f15e6acf89
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:23:17 2026 -0600

    Cambio de nombre del archivo contacto a contactoCopia

commit 4788ee1f89b81b12f9369f6cf4bf841a24e1b95e
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:18:28 2026 -0600

    Modificaciones De Contacto desde master

commit ef71179f52d2ec5ed65e6094c210a07d02520d82
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:12:32 2026 -0600

    Modificacion del index desde la Rama1

commit dd0d79971677e3be83839dfef241dd3a8610fea6
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 10:03:11 2026 -0600

    Notas agregadas V1

commit 93323067c88a1c1553435ed05cb6af8005e5144a
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 09:56:11 2026 -0600

    Agregacion de reglas de archivos ignorados

commit efa248706923852715ea80d4ef7c81ce55e9fbf1
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 09:53:49 2026 -0600

    Pie de magina de index

commit 6cd3059991fbd5297a2c3a1bdc103fac2ec08201
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 09:51:58 2026 -0600

    Agrgacion de los estilos de navegacion

commit b3f2878c492dda2fad89d1d545620bf43f554fda
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 09:49:35 2026 -0600

    Formulario para la pagina de contacto

commit 5f8c25f49faba6426a8402363aaeb604e2a021fd
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 09:48:26 2026 -0600

    Pagina de contacto agregada

commit e9382afbeb5c1213e7b51bcdc5e26050eb6e1901
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 09:46:55 2026 -0600

    Pagina de acerca modificada

commit 271e829fcf8bbb75a4c685ccd6d4ef4ffe626384
Author: sisteas03-ux <sistemas03@accounty.mx>
Date:   Tue Sep 8 09:45:36 2026 -0600

    Menu agregado


Administrator@DESKTOP-B35M9DA MINGW64 ~/documents/GiThUB/Practica (master)
$



## Rama protegida

Una rama protegida es una rama de un repositorio a la que se le aplican reglas para evitar cambios directos o accidentales.

Por ejemplo, la rama `main` puede configurarse para exigir que los cambios se realicen mediante Pull Requests y sean revisados antes de incorporarse.

Las reglas de protección ayudan a mantener la calidad del código y a evitar que modificaciones sin revisión lleguen directamente a la rama principal.

## Organización de GitHub

Una organización de GitHub es un espacio compartido que permite administrar repositorios y colaborar con otras personas.

A diferencia de una cuenta personal, una organización está pensada para equipos, proyectos, empresas o grupos que necesitan administrar conjuntamente repositorios, permisos y miembros.

Las organizaciones permiten establecer diferentes niveles de acceso para los integrantes y facilitan la administración de proyectos colaborativos.

## Deploy key

Una deploy key es una llave SSH asociada directamente con un repositorio de GitHub.

Puede utilizarse para permitir que un servidor o sistema automatizado acceda a un repositorio mediante SSH sin utilizar las credenciales personales de un usuario.

Una deploy key debe manejarse cuidadosamente porque proporciona acceso al repositorio al que está asociada. Dependiendo de su configuración puede tener permisos de lectura o también de escritura.

## Diferencia entre una llave SSH personal y una deploy key

Una llave SSH personal se utiliza para autenticar a una persona con GitHub y permitirle trabajar con los repositorios a los que tiene acceso.

Una deploy key, en cambio, está vinculada directamente a un repositorio y normalmente se utiliza para automatizaciones o servidores que necesitan acceder a ese repositorio.

Por lo tanto, no deben confundirse: una llave SSH personal identifica al usuario, mientras que una deploy key proporciona acceso específico a un repositorio.




