# Práctica 4

## Objetivo
Comprobar el rendimiento de servidores web.

## Tareas a realizar
En esta práctica se deben usar las dos herramientas para medir, primero el rendimiento de una sola máquina servidora (haciendo peticiones a la IP de la máquina 1, p.ej.), y a continuación el rendimiento de la granja web cuando usamos balanceo de carga tanto con nginx como con haproxy (haciendo las peticiones a la dirección IP del balanceador).

Realizaremos 10 mediciones para obtener media y desviación estándar con cada métrica recogida y se mostrarán los resultados en forma de tabla y gráficas para comparar los resultados obtenidos con las tres configuraciones.

## Configuración 

Para  comprobar el rendimiento de la granja web  se usa las siguientes herramientas.

- Apache Benchmark
- Siege
- OpenWebLoad

Instalamos Apache Benchmark y Siege.

 

a continuación procedo con la instalación de Siege y la generación del archivo de configuración.

##Instalamos Apache Benchmark y Siege.

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P4/1.PNG)


![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P4/instalacion%20siege.PNG)


##Resultados con Apache BenchMark y Siege

![imagen](https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P4/APACHE-HAPROXY.PNG)

![imagen] (https://github.com/NiKaJim/SWAP/blob/master/imagenes/Capturas%20P4/datos%20correctos%20siege.PNG)


Las gráficas y los datos se encuentran en los pdf adjuntos a la carpeta. 

https://github.com/NiKaJim/SWAP/tree/master/PRACTICAS/P4/Datos%20y%20graficas


