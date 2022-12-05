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
| `sudo adduser [NOMBRE]`  | Para agregar un usuario nuevo |   sudo adduser Wilson              |
| `sudo passwd [USUARIO]`  | Content |                 |
| `history`  | Content |                 |
| `crontab -e`  | Content |                 |
| `ln -s [Archivo original] [Archivo a enlazar]`  | Content |                 |
| `ln [Archivo original] [Archivo a enlazar]`  | Content |                 |
| `lsblk -o NAME,SIZE,FSTYPE,TYPE,MOUNTPOINT`  | Content |                 |
| `sudo mdadm --create --verbose /dev/md0 --level=5 --raid-devices=4 /dev/sdb /dev/sdc /dev/sdd /dev/sde `  | Content |                 |
| `sudo mkfs.ext4 -F /dev/md0`  | Content |                 |
| `whoami`  | Content |                 |
| `tail -nLineas`  | Content |                 |
| `head -nLineas`  | Content |                 |
| `more`  | Content |                 |
| `ip a`  | Content |                 |
| `hostname`  | Content |                 |
| `reboot`  | Content |                 |
| `shutdown`  | Content |                 |
| `tar -cvf archivo.tar + "nombre del archivo"`  | Content |                 |
| `tar -xvf archivo.tar `  | Content |                 |
| `chmod [Permiso] [Archivo]`  | Content |                 |
| `chown [Usuario] [Archivo]`  | Content |                 |
| `chgrp [Grupo] [Archivo]`  | Content |                 |
| `apt `  | Content |                 |
| `du "archivo" `  | Content |                 |
| `touch [nombreArchivo] `  | Content |                 |

## Comandos de Docker

|   Comandos    |  Descripción  |  Ejemplo de uso |
| ------------- | ------------- | --------------- |
| `docker run [Imagen]`  | Content  |                 |
| `docker run -ti [imagen]`  | Content  |                 |
| `sudo usermod -aG docker ${USER} & su - ${USER} `  | Content |                 |
| `sudo systemctl start docker & sudo systemctl enable docker `  | Content |                 |
| `docker search [imagen] `  | Content |                 |
| `docker pull [Imagen] `  | Content |                 |
| `docker images `  | Content |                 |
| `sudo docker ps -a `  | Content |                 |
| `sudo  docker start [ID] `  | Content |                 |
| `sudo  docker stop [ID] `  | Content |                 |
| `docker attach [contenedor] `  | Content |                 |
| `docker run -ti --rm [ID] `  | Content |                 |
| `docker rm [ID] `  | Content |                 |
| `docker info `  | Content |                 |
| `sudo docker rm $(sudo docker ps -a -f status=exited -q) `  | Content |                 |
| `docker rmi -f [Imagen] `  | Content |                 |
| `docker search linux `  | Content |                 |




