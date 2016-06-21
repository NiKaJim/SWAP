#Practica 2:  Clonacion de la informacion de un sitio web

Tenemos que configurar las maquinas para que en la red se vean entre si.
Para ello configuramos la red de cada una de ellas, nos metemos en configuracion, red y 
en redes añadimos red nat en cada una de ellas.


##Creamos un tar con ficheros locales en un equipo remoto

Procedemos a crear un fichero tar en el equipo remoto.
Creamos un fichero en un equipo remoto mediante ssh con la siguiente orden:
tar czf - directorio | ssh nika@192.168.142.129 'cat > ~/tar.tg'

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P2/m1%20www%20inicial.PNG)
![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P2/m2%20www%20inicial.PNG)

##Instalar la herramienta rsync para realizar las copias de manera incremental.

Instalamos mediante la orden:
"sudo apt-get install rsync"

Introducimos en la maquina 2 el siguiente comando para poder copiar los archivos del directorio /var/www/ de una maquina virtual a otra:
"rsync -avz -e nika@192.168.142.129:/var/www/ /var/www/"


![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P2/envio%20paquetes.PNG)

Los directorios y ficheros copiados en la máquina destino mantienen los permisos que en la máquina origen.

##Acceso sin contraseña para ssh

Mediante ssh-keygen podemos generar la clave, con la opción -t para el tipo de clave.

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P2/rsync%20maquina2.PNG)

##crontab

A continuacion vamos a realizar una tarea crontab que conecte dos maquinas mediante rsync para que realice las copias con la frecuencia
que indiquemos en crontab.

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P2/crontab.PNG)







