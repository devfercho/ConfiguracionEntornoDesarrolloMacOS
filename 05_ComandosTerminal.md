##Comandos básicos de la terminal

- clear: limbiar la terminal
- cd: (Change Directory): Moverte entre carpetas
    - cd Documents
    - cd .. -> para ir atras
    
- ls: (List) Lista todas las carpetas y archivos que hay dentro de la ubicación en la que estemos.
- ls -a: Lista todo, incluyendo lo oculto
- open: Abre un archivo con el programa predeterminado, si el archivo o carpeta tiene espacios, encierra el nombe en comillas dobles
- sudo: permite ejecutar cualquier comando como super administrador
- reset: Reinicia la terminal
- ctrl + c: Detiene cualquier proceso que se esté ejecutando en la terminal.
- pwd: muestra la ruta del directorio actual
- mkdir nombre_del_dir: crea un nuevo directorio
- rm archivo: borra el archivo especifico
- rm -r dir: borra el directorio especificado
- rm -f archivo: borra de manera forzada un archivo
- rm -rf dir: borra el directorio de manera forzada
- cp -r archivo1 archivo2: copia el archivo1 en al archivo2 
- cp -r dir1 dir2: copia el directorio1 al directorio2; crea el directorio2 en caso de que no exista (sustituir la variable dir por el nombre del directorio)
-  mv archivo1 archivo2: puede ser utilizado para cambiar el nombre o mover el archivo1 al archivo2. Si archivo2 es un directorio existente, mueve el archivo1 dentro del directorio “archivo2” (sustituir la variable archivo por el nombre del archivo)
-  ln -s archivo link: crea un enlace simbólico (acceso directo) para un archivo (sustituir la variable archivo por nombre del archivo y el enlace con el nombre que tendrá el acceso directo)
-  touch archivo: crea o actualiza el archivo (sustituir la variable archivo por el nombre del archivo)
-  cat > archivo: redirige la entrada estándar a un archivo (sustituir la variable archivo por el nombre del archivo)
-  more archivo: muestra el contenido de un archivo
-  **head archivo: **muestra las 10 primeras líneas de un archivo
-  tail archivo: muestra las últimas 10 líneas de un archivo
-  tail -f archivo: muestra el contenido de un archivo mientras se actualiza (aumenta de tamaño), a partir de las últimas 10 líneas.

##Administración de procesos
- ps: muestra los procesos de usuario activos en tiempo real
- top: muestra todos los procesos que se ejecutan en tiempo real
- kill pid: mata un proceso específico por el número ID (sustituir pid por el número de proceso)
- killall proc: mata todos los procesos con el nombre especificado (sustituir proc por el nombre del proceso)
- bg: lista de trabajos parados o en segundo plano
- fg: trae el trabajo más reciente a primer plano
- fg trab: trae el trabajo “trab” a primer plano (reemplazar trab por el nombre del proceso)

##Comandos para búsquedas
- grep secuencia archivos: búsqueda de la secuencia de los archivos (sustituir la secuencia y archivos por los valores correspondientes a la investigación)
- **grep-r secuencia dir: ** búsqueda de forma recursiva por la secuencia en el directorio dir
- comando | grep secuencia: busca por la secuencia en la salida del comando (sustituir comando y secuencia de acuerdo con los valores a ser buscados)
- locate archivo: encuentra todas las instancias de un archivo (sustituir la variable archivo por el nombre del archivo)

##Información del sistema

- date: muestra la fecha y la hora actual
- cal: muestra un calendario del mes actual
- uptime: muestra el tiempo de actividad del sistema
- w: muestra quién está en línea
- whoami: muestra quién está conectado
- finger usuario: muestra la información del usuario
- uname -a: muestra la información de núcleos
- cat /porc/cpuinfo: muestra la información de la CPU
- cat /proc/meminfo: muestra la información de la memoria
- man comando: abre el manual del comando especificado (sustituir la variable comando por el nombre del comando que se quiere conocer)
- df: muestra el uso del disco
- du: muestra el uso del espacio en un directorio
- free: muestra el uso de la memoria y swap
- whereis aplicación: muestra las posibles ubicaciones de la aplicación (reemplazar aplicación por el nombre del programa)
- which aplicación: muestra qué aplicación se ejecutará por defecto (reemplazar aplicación por el nombre del programa)

##Compresión de archivos

- tar cf paquete.tar archivos: crea un paquete TAR (nombrado paquete.tar) con los archivos especificados (sustituir la variable archivos por el nombre del archivo)
- tar xf paquete.tar: extrae los archivos de paquete.tar (reemplazar la variable paquete.tar por el nombre del archivo)
- tar czf pacote.tar.gz archivos: crea un paquete TAR (nombrado pacote.tar.gz) con la compresión GZip
- tar xzf pacote.tar.gz: extrae un paquete TAR (nombrado pacote.tar.gz) con la compresión GZip
- tar cjf paquete.tar.bz2: crea un paquete TAR (nombrado paquete.tar.bz2) con la compresión BZip2
- tar xjf paquete.tar.bz2: extrae un paquete TAR con la compresión BZip2
- gzip archivo: comprime un archivo y el nombre a archivo.gz (sustituir la variable archivo por el nombre del archivo)
- gzip -d archivo.gz: descomprime archivo.gz a un archivo (sustituir la variable archivo.gz por el nombre del archivo)