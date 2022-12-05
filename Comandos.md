# Comandos de Sistemas Operativos 4/12/2020

### Estudiante: Wilson Gong Wu

## Comandos

|   Comandos    |  Descripción  |  Ejemplo de uso |
| ------------- | ------------- | --------------- |
| `ls`  | Content  | Es para ver la lista de archivos 
y directorios en el directorio actual | ls `output: Comandos.md  README.md`
| `pwd`  | Content  |                 |
| `cd`  | Content  |                 |
| `nano`  | Content  |                 |
| `mkdir`  | Content |                 |
| `rm`  | Content |                 |
| `clear`  | Content  |                 |
| `htop`  | Content |                 |
| `ps -aux`  | Content |                 |
| `pstree`  | Content |                 |
| `kill -9 [PID]`  | Content |                 |
| `pkill [PID]`  | Content |                 |
| `sudo apt update && sudo apt upgrade`  | Content  |                 |
| `man`  | Content |                 |
| `sudo su`  | Content |                 |
| `exit`  | Content |                 |
| `more`  | Content |                 |
| `cp`  | Content |                 |
| `mv`  | Content |                 |
| `sudo adduser [NOMBRE]`  | Content |                 |
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


