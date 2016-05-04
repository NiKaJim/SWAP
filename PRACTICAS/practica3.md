# Práctica 3  Balanceo de Carga


Vamos a configurar las máquinas virtuales para tener dos servidores web y otra funcione como balanceador de carga por software.

## Tareas a realizar

1. Crear una M3 y configurarla SIN Apache.
2. Poner SSH
2. Instalar el software nginx como balanceador de carga.
3. Instalar el haproxy como balanceador de carga.
4. Opcional: Instalar ZenLoadBalancer


Tras crear la nueva maquina SIN APACHE, procedemos a instalar el software Nginx mediante los comandos:

Apt-get install nginx

Y procedemos a configurar el archivo "default.conf" dentro del directorio nginx.
Importamos la clave del repositorio software
Añadimos los servidores apaches de las otras maquinas virtuales. 

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P3/CAPTURAS/2.PNG)

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P3/CAPTURAS/archivo%20conf.PNG)

Lanzamos el servicio mediante la orden

$ service nginx restart

Y si no hay ningún fallo podremos comprobar el funcionamiento del balanceador. 

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P3/CAPTURAS/comprobacion%20nginx.PNG)


Ahora vamos a configurarla para instalar el balanceador haproxy.

$ apt-get install haproxy
```
Confirmamos la ip donde tenemos el balanceador.
Modificamos el archivo /etc/haproxy/haproxy.cfg

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P3/CAPTURAS/haproxy1.PNG)

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P3/CAPTURAS/haproxy2.PNG)


Y comprobamos el funcionamiento del balanceador.

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P3/CAPTURAS/haproxy3.PNG)

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P3/CAPTURAS/comprobacion%20haproxy.PNG)



