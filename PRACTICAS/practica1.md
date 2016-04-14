# # Práctica 1.  Preparación de las herramientas

** Por Mónica Jiménez Montañés**

# Instalación de Máquinas Virtuales

	En mi caso voy a trabajar sobre VMWARE ya que me resulta más cómodo.

1.  Descarga del software

[web vmware] (http://www.vmware.com/products/player/)


2. Descarga del sistema operativo, en nuestro caso trabajaremos con Ubuntu Server.

[web ubuntu] (http://www.ubuntu.com/download/server )


3. Realizar la instalación de 2 maquinas virtuales con el sistema operativo indicado anteriormente. Podemos tener el detalle de la instalación en el siguiente enlace de un servidor completo con LAMP.

[web instalacion] (http://www.ubuntugeek.com/step-by-step-ubuntu-12-04-precise-lamp-server-setup.html )

o también podemos realizar la instalación mediante el comando:

*sudo apt-get install apache2 mysql-server php5 libapache2-mod-php5 php5-mysql *

4. Terminada la instalación comprobaremos la versión y que el servidor está ejecutándose mediante la orden:

*apache2 -v*
 
*ps aux | grep apache *


![imagen] (https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P1/version%20apache.PNG)
