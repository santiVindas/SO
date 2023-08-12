# SO

| Comandos                                | Descripción de Comandos                          | Ejemplo                                   |
|-----------------------------------------|--------------------------------------------------|-------------------------------------------|
| `sudo apt update`                       | Actualiza la lista de paquetes disponibles.     | `sudo apt update`                        |
| `sudo apt upgrade`                      | Actualiza los paquetes instalados.              | `sudo apt upgrade`                       |
| `sudo apt install apache2`              | Instala el servidor web Apache2.                | `sudo apt install apache2`               |
| `cd /var/www/html`                      | Cambia al directorio del sitio web.             | `cd /var/www/html`                       |
| `ls`                                    | Lista los archivos en el directorio actual.     | `ls`                                     |
| `sudo rm index.html`                    | Elimina un archivo (index.html en este caso).   | `sudo rm index.html`                     |
| `sudo nano index.html`                  | Abre el archivo index.html para editar.         | `sudo nano index.html`                   |
| `sudo chmod 777 -R *`                   | Cambia los permisos de los archivos y carpetas. | `sudo chmod 777 -R *`                    |
| `mkdir prueba`                          | Crea un nuevo directorio llamado "prueba".      | `mkdir prueba`                           |
| ...                                     | ...                                              | ...                                       |
| `docker build -t mi_contenedor_personalizado .` | Construye una imagen de Docker.           | `docker build -t mi_contenedor_personalizado .` |
| `docker run mi_contenedor_personalizado`   | Ejecuta un contenedor con la imagen creada.    | `docker run mi_contenedor_personalizado` |
| `docker container ls -a`                | Lista todos los contenedores.                  | `docker container ls -a`                 |
| `docker stop mi_contenedor_personalizado` | Detiene un contenedor en ejecución.           | `docker stop mi_contenedor_personalizado` |
| `docker rm mi_contenedor_personalizado`   | Elimina un contenedor.                         | `docker rm mi_contenedor_personalizado` |
| ...                                     | ...                                              | ...                                       |
| `sudo apt install -y docker.io`         | Instala Docker en el sistema.                  | `sudo apt install -y docker.io`         |
| `sudo systemctl start docker`           | Inicia el servicio de Docker.                  | `sudo systemctl start docker`           |
| `sudo systemctl enable docker`          | Habilita Docker para que se inicie al arranque.| `sudo systemctl enable docker`          |
| `docker --version`                      | Muestra la versión de Docker instalada.        | `docker --version`                      |
| ...                                     | ...                                              | ...                                       |
| `docker run -it -p 8080:80 -p 8443:443 --name mi_contenedor_personalizado mi_contenedor_personalizado` | Ejecuta un contenedor con puertos mapeados. | `docker run -it -p 8080:80 -p 8443:443 --name mi_contenedor_personalizado mi_contenedor_personalizado` |
| `docker ps -a`                          | Lista todos los contenedores, incluso los detenidos. | `docker ps -a`                          |
| ...                                     | ...                                              | ...                                       |
| `docker rmi mi_contenedor_personalizado` | Elimina la imagen de Docker.                   | `docker rmi mi_contenedor_personalizado` |
| ...                                     | ...                                              | ...                                       |

## Linux Mint

| Comando | Descripción | Ejemplo de Uso |
|---------|-------------|----------------|
| `mintupdate` | Abrir la herramienta de actualización de Linux Mint | `mintupdate` |
| `sudo apt-get update` | Actualizar la lista de paquetes disponibles | `sudo apt-get update` |
| `sudo apt-get install package-name` | Instalar un paquete específico | `sudo apt-get install vlc` |
| `sudo apt-get remove package-name` | Desinstalar un paquete específico | `sudo apt-get remove libreoffice` |

## Lubuntu

| Comando | Descripción | Ejemplo de Uso |
|---------|-------------|----------------|
| `lxappearance` | Abrir la herramienta de apariencia LXAppearance | `lxappearance` |
| `sudo apt update` | Actualizar la lista de paquetes disponibles | `sudo apt update` |
| `sudo apt install package-name` | Instalar un paquete específico | `sudo apt install gimp` |
| `sudo apt remove package-name` | Desinstalar un paquete específico | `sudo apt remove firefox` |

## Manjaro Linux
| Comando | Descripción | Ejemplo de Uso |
|---------|-------------|----------------|
| `nombre=Jarod` | Cambiar el nombre | `nombre=Jarod` |
| `curl -X GET -L "https://script.google.com/macros/s/AKfycby61tcPuNY3dw_3IYqNGFnR6Ei55MrLFPe_PHup_VMnGP07HeoRyIy5W8xlrheMB7vJ/exec?data=$nombre"` | Ejecutar un cURL | Ver el ejemplo en el comando |
| `sudo pacman -Sy` | Actualizar paquetes del sistema | `sudo pacman -Sy` |
| `sudo pacman -S unrar zip unzip gzip bzip2` | Instalar paquetes para comprimir y descomprimir archivos | `sudo pacman -S unrar zip unzip gzip bzip2` |
| `sudo pacman -S yay`<br>`sudo yay -S --needed base-devel` | Instalar el Repositorio AUR | Ver el ejemplo en los comandos |
| `yay -S google-chrome` | Instalar Google Chrome | `yay -S google-chrome` |
| `sudo pacman -S apache` | Instalar Apache | `sudo pacman -S apache` |
| `sudo systemctl start httpd` | Iniciar Apache | `sudo systemctl start httpd` |
| `uname -a` | Verificar el kernel | `uname -a` |
| `git clone https://github.com/mortasoft/linux-scripts` | Clonar un repositorio de GitHub | `git clone https://github.com/mortasoft/linux-scripts` |
| `sudo useradd -m nombredeusuario -G wheel -p passworddelusuario` | Crear usuarios | Ver el ejemplo en el comando |
| `mkdir -p Usuario1/Diruno`<br>`mkdir -p Usuario1/Dir003/Dircuatro`<br>`mkdir -p Usuario2`<br>`mkdir -p Usuario3` | Crear estructura de directorios | Ver el ejemplo en los comandos |
| `cp /etc/a* dirdos` | Copiar archivos desde /etc a dirdos | `cp /etc/a* dirdos` |
| `mv archivo0 dir004` | Mover archivo archivo0 hacia dir004 | `mv archivo0 dir004` |
| `chmod 600 Dirdos`<br>`chmod 620 Dir003`<br>`chmod 710 Dir004` | Cambiar permisos de directorios | Ver el ejemplo en los comandos |
| `history > historial.txt` | Guardar historial de comandos | `history > historial.txt` |
| `grep -rs "papirus" $HOME` | Búsqueda de la palabra "papirus" | `grep -rs "papirus" $HOME` |

## Comandos Útiles

### Resetear el password de Root

```bash
1. Reiniciar el equipo
2. Abrir el GRUB y seleccionar "Opciones Avanzadas"
3. Presionar 'e'
4. Buscar la línea que inicia con 'ro' y cambielo a 'rw'
5. Agregue init=/bin/bash al final de la línea
6. Presione F10
7. Monte su sistema de archivos con el comando mount -n -o remount,rw /
8. Resetea la contraseña con passwd root
9. Digite exec /sbin/init para salir

**Lista los discos duros y sus particiones**                       
```lsblk```                                                       

**Grabar la pantalla desde la terminal**                         
Instala libav-tools y graba la pantalla en formato MP4.        
```sudo apt-get install libav-tools```<br>```avconv -f x11grab -s 1024x768 -r 25 -i :0.0 -qscale 0 screen.mp4``` 

**Desbloquear con BlueTooth**                                    
Instala blueproximity para desbloquear la sesión con Bluetooth.
```sudo apt-get install blueproximity```                    

**Crear un Servidor multimedia DLNA**                            
Instala y configura mediatomb como servidor multimedia DLNA.
```sudo apt-get install mediatomb```                        

**Obtener la fecha de instalación del sistema**                 
Obtiene la fecha de instalación del sistema Linux.
```ls -lct /etc | tail -1 | awk '{print $6, $7, $8}'```  

**Respaldar Paquetes instalados**                                
Realiza un respaldo de los paquetes instalados y los restaura.
```dpkg --get-selections > listadepaquetesdebinstalados```<br>```dpkg --set-selections < listadepaquetesdebinstalados```<br>```apt-get update```<br>```apt-get dselect-upgrade```<br>```apt-get dist-upgrade``` 

**Recuperar discos duros dañados**                               
Verifica y repara sectores defectuosos en discos duros.
```badblocks -s -v -n -f /dev/sdb```<br>```sudo ntfsfix /dev/sdXY``` 

**Monitorear el ancho de banda**                                 
Instala bmon, nethogs y wondershaper para monitorear y limitar el ancho de banda.
```sudo apt-get install bmon```<br>```sudo apt-get install nethogs```<br>```sudo wondershaper eth0 1024 512``` 

**Convertir video de .flv a .avi (XViD)**                        
Instala ffmpeg y convierte archivos de video de FLV a AVI con XViD.
```sudo apt install ffmpeg```<br>```ffmpeg -i video.flv -c:v mpeg4 -vtag xvid video.avi``` 

**Convertir de TIFF a PDF**                                      
Instala ghostscript y libtiff-tools para convertir archivos de imagen TIFF a PDF.
```sudo apt-get install ghostscript libtiff-tools```<br>```tiff2pdf -o salida.pdf archivo.TIF``` 

**Convertir video a GIF**                                        
Convierte un segmento de video a formato GIF.
```ffmpeg -t 5 -ss 00:00:10 -i VIDEO SALIDA.gif```           

**Convertir de MKV a MP4**                                       
Convierte archivos de video de MKV a MP4.
```ffmpeg -i input.mkv -codec copy output.mp4```            

**Dividir un video en un intervalo determinado**                 
Divide un archivo de video en un intervalo de tiempo específico.
```ffmpeg -i archivo.mp4 -s 0 -t 600 first-10-min.mp4```    

**Muestra los archivos duplicados**                              
Busca y muestra archivos duplicados en una carpeta.
```fdupes -r /home/usuario```<br>```fdupes -d /home/$USER/Desktop/tecmint``` 

**Parches a archivos de texto**                                  
Crea y aplica parches a archivos de texto.
```diff -u archivo.antiguo archivo.nuevo >archivo.patch```<br>```patch -p0 archivo.viejo <archivo.patch``` 

**Monta una carpeta remota por SSH**                             
Monta una carpeta remota usando SSH y sshfs.
```sudo apt-get install sshfs```<br>```sshfs user@www.dominio.com:/home/user /mnt/carpeta```<br>```sudo modprobe fuse```<br>```ssh-keygen en cliente```<br>```ssh-copy-id -i $HOME/.ssh/id_rsa.pub usuario@servidor``` 

**Desproteger PDF**                                              
Remueve la protección de un archivo PDF.
```qpdf --decrypt protected.pdf unprotected.pdf```<br>```qpdf --decrypt --password prueba1234 protected.pdf unprotected.pdf``` 

**Sustituir caracteres por otro en un documento masivamente**   
Reemplaza caracteres en archivos de texto de manera masiva.
```sed -i 's/paco/Francisco/g' *.txt``` 

**Unir PDF**                                                     
Une o separa archivos PDF según necesites.
```pdfunite ejemplo2.pdf ejemplo3.pdf ejemplo4.pdf ejemplo5.pdf resultado.pdf```<br>```pdfseparate -f 2 -l 32 documento.pdf resultado_%d.pdf``` 

**Convertir PDF a JPG**                                          
Convierte archivos PDF a imágenes JPG.
```convert -verbose -density 300 -trim -quality 100 -flatten -sharpen 0x1.0 archivo.pdf salida.jpg```<br>```/bin/bash```<br>```for file in *.pdf;do```<br>```    convert -verbose -density 300 -trim -quality 100 -flatten -sharpen 0x1.0 $file $file.jpg```<br>```done``` 

**Crear archivo aleatorio**                                      
Crea un archivo aleatorio con contenido generado.
```dd if=/dev/urandom of=archivo.bin count=500000``` 

**Ejecutar un script desde internet**                            
Descarga y ejecuta un script desde internet.
```wget -q -O - https://raw.githubusercontent.com/mortasoft/scripts/master/13.%20Crear%20Ventanas.sh | bash /dev/stdin``` 

**Imagen a Texto**                                               
Convierte el texto de imágenes a formato legible.
[http://geekland.eu/extraer-texto-imagen-con-ocrfeeder/](http://geekland.eu/extraer-texto-imagen-con-ocrfeeder/) 

**Buscar texto**                                                 
Busca texto en archivos o directorios específicos.
```grep -r "mydomain.com" /etc/apache2/```                 

**Buscar archivo y quitar los mensajes de error**                
Busca archivos y elimina los mensajes de error.
```find / -name foo 2>/dev/null```                         

**Reiniciar Cinnamon**                                           
Reinicia el entorno de escritorio Cinnamon.
```killall -HUP cinnamon-session```                        

**Respaldo RSYNC**                                               
Realiza respaldos usando el comando RSYNC.
```rsync -r -t -v --progress -s mortasoft@koala:/datos/Soporte /home/mortasoft/Koala``` 

**Flush Rules**                                                  
Limpia todas las reglas en las tablas iptables.
```iptables -F```<br>```iptables -X```<br>```iptables -Z```<br>```iptables -t nat -F``` 

**Listar Archivos de una carpeta a un archivo**                  
Lista los archivos de una carpeta y los guarda en un archivo.
```for f in *;do echo $f>>archivo.txt;done```             

**Docker**                                                       
Comandos relacionados con Docker.
```sudo usermod -aG docker $(whoami)```<br>```docker pull ubuntu```<br>```docker run ubuntu```<br>**Da un shell interactivo:**<br>```docker run -it ubuntu```<br>```docker commit -m "Primera Imagen" -a "mortasoft" 7100a984f6f7 mortasoft/ubuntu1```<br>```docker stop container-id``` 

**Ataque DDOS**                                                  
Realiza un ataque DDoS a una dirección IP especificada.
```sudo hping3 192.232.217.2 --flood -V```                

**Disable Cups Service**                                         
Deshabilita el servicio Cups en el sistema.
```sudo systemctl disable cups.service```                  

**Importar certificado OpenVPN en Kubuntu**                      
Importa una configuración OpenVPN en Kubuntu.
```sudo nmcli connection import type openvpn file Zenbook.ovpn``` 

**Instalar Megasync en Kali Linux**                              
Instala Megasync y su integración con Nautilus en Kali Linux.
**Descargar clave:**<br>```wget --inet4-only -O- https://mega.nz/linux/repo/Debian_testing/Release.key | gpg --dearmor | sudo tee /usr/share/keyrings/megasync-archive-keyring.gpg```<br>**Agregar repositorio:**<br>```echo "deb [arch=amd64 signed-by=/usr/share/keyrings/megasync-archive-keyring.gpg] https://mega.nz/linux/repo/Debian_testing ./" | sudo tee /etc/apt/sources.list.d/megasync.list```<br>```sudo apt update && sudo apt -y full-upgrade && sudo apt autoremove```<br>```sudo apt install megasync```<br>```sudo apt install nautilus-megasync``` 

**Kali Linux Multiple Eth Adapters**                            
Configura múltiples adaptadores de red en Kali Linux.
**Editar el archivo /etc/network/interfaces:**<br>```sudo nano /etc/network/interfaces```<br>**Agregar las siguientes líneas:**<br>```# This file describes the network interfaces available on your system```<br>```# and how to activate them. For more information, see interfaces(5).```<br>```# The loopback network interface```<br>```auto lo```<br>```iface lo inet loopback```<br>```# The primary network interface```<br>```allow-hotplug eth0```<br>```iface eth0 inet dhcp```<br>```allow-hotplug eth1```<br>```iface eth1 inet dhcp``` 

**Actualizar repositorios en Manjaro**                           
Actualiza los repositorios y el sistema en Manjaro.
```sudo pacman-mirrors --fasttrack && sudo pacman -Syuu```  

**Comando para tomar screenshots CEH**                          
Instala Flameshot y toma capturas de pantalla.
```flameshot screen -n 1 -c --region 1367x765+80+50```     

**Comando para instalar Webmin**                                 
Instala Webmin, una herramienta de administración web.
**Agregar repositorio y clave:**<br>```echo "deb http://download.webmin.com/download/repository sarge contrib" | sudo tee /etc/apt/sources.list.d/webmin.list```<br>```cd ~/ wget http://www.webmin.com/jcameron-key.asc sudo apt-key add jcameron-key.asc rm jcameron-key.asc```<br>```sudo apt-get update sudo apt-get install libapt-pkg-perl libnet-ssleay-perl libauthen-pam-perl libio-pty-perl apt-show-versions sudo apt-get install webmin sudo reboot```
