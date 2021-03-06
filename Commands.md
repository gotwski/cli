# :rocket: Comandos

#### :minidisc: Listado de archivos y navegación
* `pwd`: Muestra la ruta en la que te encuentras actualmente.
* `ls`: Lista archivos de un directorio.
* `ls -l`: Lista archivos de un directorio con formato de lista.
* `ls -lh`: Lista archivos de un directorio con formato de lista y humanamente legible :bowtie:
* `cd`: Navega al directorio Home.
* `cd [dir]`: Navega a un directorio específico.
* `cd ..`: Regresa a la directorio anterior.

#### :floppy_disk: Crear/Mover/Copiar directorios o archivos
* `mv [dir|arch] [dir destino]`: Mueve un directorio o archivo a un directorio específico.
* `mv ~/[dir|arch] ./`: Mueve un directorio o archivo que se encuentra alojado en `home` hacia el directorio en el que te encuentras.
* `cp [dir|arch] [dir destino]`: Crea una copia del directorio o archivo original en un directorio específico.

#### :file_folder: Renombrar directorios o archivos
* `mv [dir] [new_dir]`: Cambia el nombre de un directorio.
* `mv [arch] [new_arch]`: Cambia el nombre de un archivo.

#### :open_file_folder: Tocar/Crear direcorios o archivos
* `mkdir [arch]`: Crea un directorio con un nombre específico.
* `touch [arch]`: Crea un archivo con un nombre específico.

#### :bomb: Eliminar archivos o directorios
* `rm [arch]`: Elimina un archivo de nombre específico.
* `rm [dir]/*`: Elimina todos los archivos dentro de un directorio.
* `rm -rf [dir]`: Elimina todo el contenido del directorio y el directorio mismo.

#### :crystal_ball: Miscelanea
* `man [command]`: Muestra la documentación de un comando específico.
* `open -a [app] [arch]`: Abre un archivo específico con una aplicación específica.
* `bc`: Te permite realizar cálculos matemáticos.
* `bc [arch]`: Realiza los cálculos de las operaciones escritas en un archivo.
* `cat [arch]`: Imprime el contenido de un archivo.
* `more [arch]`: Imprime/pagina el contenido de un archivo.
* `head`: Imprime las primeras 10 líneas de un archivo.
*  `tail`: Imprime las últimas 10 líneas de un archivo.
* `wc [arch]`: Imprime el número de líneas, palabras y caracteres de un archivo.
* `vim`: Editor de texto disponible en la terminal.
* `date`: Imprime la fecha actual.
* `uname` : Imprime el nombre del Sistema Operativo.
* `expr [n+n]`: Evalua expresiones matemáticas.
* `whoami`: Imprime el nombre de usuario actual.

#### :mag_right: Procesos
* `echo`: Imprime exactamente lo que le pases como argumento.
* `echo $PATH`: Imprime el contenido de la variable `$PATH`, es decir, las rutas de directorios que contienen comandos ejecutables.
* `/usr/bin`: Ejemplo de directorio que contiene un par de comandos ejecutables.
* `which [command]`: Imprime la ruta desde la que se está ejecutando un commando específico.
* `top`: Muestra una lista de todos los procesos en ejecución, su commando y PID.
* `kill -9 [command]`: Mata un proceso específico en ejecución.

#### :japanese_ogre: Algo de diversión
* `rev [arch]`: Invierte todas las palabras escritas en un archivo.
* `yes [text]`: Texto infinitoooooooo.
* `fourtune`: Galletitas de la fortuna al azar.
* `sl`: Una locomotora atravesará tu terminal cuando por error escribas `sl` y no `ls`.
* `figlet -f [font] [text]`: Imprime en ascii lo que quieras leer en la terminal.
* `cowsay [text]`: Imprime en ascii una vaca que habla.
* `toilet --gay [text]`: Imprime en ascii arcoíris lo que quieras leer en la terminal.
* `aafire`: ¡Prende una fogata!
* `oneko`: Un gatito tratará de alcanzar tu cursor.
* `cmatrix`: Tu terminal al estilo matrix.
* `rig`: Imprime identidades fake al azar.

#### :computer: Entrada, Salida y Error estándar.
* `Standar Input` o `stdin`: Es la fuente de entrada de datos para programas ejectudados desde la línea de comandos, ej. teclado.
* `Standar Output` o `stdout`: Salida estándar que imprime datos como resultado de ejecutar un programa, ej. terminal.
* `Standar Error` o `stderr`: Imprime errores mediante una salida estándar como resultado de un fallo al ejecutar un programa.
* `echo "2 * 3" | bc -q `: Usando pipe podemos tomar la salida de un comando como entrada de otro.
* `echo Ahoy, World! > [arch]`: Usando `mayor-que` podemos guardar la salida de un comando en un archivo.
* `bc -q < [arch]`: Usando `menor-que` podemos tomar como entrada de datos un archivo, etc.

#### :microscope: Búsqueda en archivos o directorios.
* `grep [pattern]`: Encuentra coincidencias con base en un patrón específico.
* `grep ^[word] < [arch]`: Imprime todas las líneas que empiezan con una palabra en específico.
* `grep [word]$ < [arch]`: Imprime todas las líneas que terminan con una palabra en específico.
* ej. `cat lorem.txt | grep ^Lorem > output-lorem.txt`: Guarda en un achivo todas las líneas que empiecen con la palabra `Lorem`
* `find`: Busca archivos con base en un patrón o nombre específico.
* ej. `find . -name '*.md' -type f`: Busca coincidencias que en su extensión sean `.md`.
* ej. `find . -name 'README' -type f -exec mv {} {}.md \;'`: Busca todos los archivos `README` y les agrega la extensión `.md`

#### :hand: Permisos en archivos o directorios.
* `chmod [num] [arch]`: Modifica los permisos de un archivo o directorio.
* `-rwxrwxrwx`: Hace referencia a los permisos de lectura, escritura y ejecución de un archivo o directorio.
* `-[rwx][rwx][rwx]`: Permisos por bloque 1-Usuario, 2-Grupo, 3-Público.

#### :penguin: Shell Scripting
* `#!/bin/bash`: Le dice al shell qué programa interpretará el script.
