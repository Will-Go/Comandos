# Comandos de Sistemas Operativos 4/12/2022

### Estudiante: Wilson Gong Wu

## Comandos

|   Comandos    |  Descripción  |  Ejemplo de uso |
| ------------- | ------------- | --------------- |
| `ls`  | Es para ver la lista de archivos y directorios en el directorio actual  | ls `output: Comandos.md  README.md` | 
| `pwd`  | Ver la ruta en la esta actualmente  | pwd `output: /home/prueba/Comandos`  |
| `cd [Directorio]`  | Moverse de directorio  | cd /home/ |
| `nano [Archivo]`  | Editor de texto de archivos  | nano comandos.md   |
| `mkdir [Nombre]`  | Crear un directorio |  mkdir carpeta01         |
| `rm [archivo]`  | Borrar un archivo | rm README.md      |
| `rm -d [directorio]`  | Borrar un directorio | rm -d carpeta01 |
| `clear`  | Limpiar la terminal  |  clear "Se limpia la consola"            |
| `htop`  | Ver los procesos actuales interactivamente |  htop "Muestra procesos"     |
| `ps -aux`  | Ver los procesos, pero en el instante en el que se ejecuto el comando |  ps -aux "Muestra procesos"               |
| `pstree`  | Ver los procesos, pero en la instante y en forma de arbole |  pstree "Mueestra procesos"               |
| `kill -9 [PID]`  | Mata la señal del proceso  |  kill -9 18775               |
| `pkill [PID]`  | Mata el proceso  |  pkill 18775               |
| `sudo apt update && sudo apt upgrade`  | Actualiza el repositorio y actualiza el sistema  |  sudo apt update && sudo apt upgrade               |
| `man`  | Da instrucciones sobre un comando en especifico | man ls                |
| `sudo su`  | Cambia a un usuario root | sudo su                |
| `exit`  | Sales de la terminal o usuario | exit                |
| `more [archivo]`  | Despliega un output de un comando o contenido de archivo en paginas navegables | more /etc/ssh/sshd_config                |
| `cp [archivo] [directorio]`  | Para copiar y pegar archivos en otros directorios | cp comandos.md /home/                |
| `mv [archivo] [directorio]`   | Para mover archivos a otros directorios | mv comandos.md /home/prueba/Comandos                |
| `sudo adduser [NOMBRE]`  | Para agregar un usuario nuevo |   sudo adduser fredo              |
| `sudo passwd [USUARIO]`  | Para cambiar la contraseña de un usuario |  sudo passwd fredo                |
| `history`  | Para mostrar el registro de comandos de usuario actual | history                |
| `crontab -e`  | Para editar el archivo de crontab |   crontab -e              |
| `ln -s [Archivo original] [Archivo a enlazar]`  | Para hacer enlaces suaves |  ln -s /home/prueba/hola.sh /home/prueba/Comandos/               |
| `ln [Archivo original] [Archivo a enlazar]`  | Para hacer enlaces duros |  ln /home/prueba/hola.sh /home/prueba/Comandos/               |
| `lsblk -o NAME,SIZE,FSTYPE,TYPE,MOUNTPOINT`  | Para ver los discos actuales de la maquina | lsblk -o NAME,SIZE,FSTYPE,TYPE,MOUNTPOINT                |
| `sudo mdadm --create --verbose /dev/md0 --level=5 --raid-devices=4 /dev/sdb /dev/sdc /dev/sdd /dev/sde `  | Crea un RAID5 con 4 discos | sudo mdadm --create --verbose /dev/md0 --level=5 --raid-devices=4 /dev/sdb /dev/sdc /dev/sdd /dev/sde                |
| `sudo mkfs.ext4 -F /dev/md0`  | Para hacer el grupo de discos |  sudo mkfs.ext4 -F /dev/md0               |
| `whoami`  | Para saber en que usuario estoy actualmente |  whoami               |
| `tail -nLineas [archivo]`  | Para mostrar una cantidad especifica de lines alfinal de un archivo | tail -10 Comandos.md                 |
| `head -nLineas`  | Para mostrar una cantidad especifica de lines alfinal de un archivo |  head -10 Comandos.md                |
| `ip a`  | Para mostrar informacion de la red |   ip a              |
| `hostname`  | Para mostrar el nombre de la maquina | hostname                |
| `reboot`  | Reinicia la maquina |   reboot              |
| `shutdown`  | Apaga la maquina |  shutdown               |
| `tar -cvf archivo.tar + "nombre del archivo"`  | Comprime un archivo y directorios | tar -cvf comandos.tar + "Comandos"                |
| `tar -xvf archivo.tar `  | Descomprime un archivo.tar |  tar -xvf comandos.tar               |
| `chmod [Permiso] [Archivo]`  | Cambia permisos a un archivo | chmod 777 hola.sh               |
| `chown [Usuario] [Archivo]`  | Cambia de dueño un archivo | chown comandos.md fredo                |
| `chgrp [Grupo] [Archivo]`  | Cambia de grupo el archivo | chgrp corleones comandos.md                |
| `du "archivo" `  | Mostrar el tamaño de un archivo |  du comandos.md               |
| `touch [nombreArchivo] `  | Crea un archivo | touch libros.txt                |

## Comandos de Docker

|   Comandos    |  Descripción  |  Ejemplo de uso |
| ------------- | ------------- | --------------- |
| `sudo systemctl start docker & sudo systemctl enable docker `  | Comienza el docker  |  sudo systemctl start docker & sudo systemctl enable docker               |
| `docker run [Imagen]`  | Crea un contenedor con la imagen deseada  | docker run ubuntu                |
| `docker run -ti [imagen]`  | Crea un contenedor con la imagen deseada, de forma interactiva y directamente en la terminal  | docker run -ti ubuntu                 |
| `sudo usermod -aG docker ${USER} & su - ${USER} `  | Hace que el comando docker no sea necesario ejecutarse con sudo | sudo usermod -aG docker fredo & su - fredo  |
| `docker search [imagen] `  | Busca imagenes relacionadas  | docker search linux                |
| `docker pull [Imagen] `  | Instala la imagen  | docker pull ubuntu                |
| `docker images `  | Muestra las imagenes instaladas | docker images                |
| `sudo docker ps -a `  | Muestra todos los contenedores e informacion de ellos  |   sudo docker ps -a               |
| `sudo  docker start [ID] `  | Empieza un contenedor | sudo  docker start ad33d63a2f7i                |
| `sudo  docker stop [ID] `  | Apaga un contenedor |  sudo  docker stop ad33d63a2f7i                |
| `docker attach [contenedor] `  | Se mete en la terminal de un contenedor | docker attach ad33d63a2f7i                |
| `docker run -ti --rm [imagen] `  | Comienza un contenedor, interactivamente y en la terminal, pero cuando cierra la terminnal se borra el contenedor |                docker run -ti --rm ubuntu |
| `docker rm [ID] `  | Borra el contenedor | docker rm  ad33d63a2f7i              |
| `docker rmi -f [Imagen] `  | Borra una imagen | docker rmi -f ubuntu                |
| `docker info `  | Muestra la informacion de la maquina | docker info                |
| `sudo docker rm $(sudo docker ps -a -f status=exited -q) `  | Borra todos los contenedores que esten en estado apagado | sudo docker rm $(sudo docker ps -a -f status=exited -q)                |






