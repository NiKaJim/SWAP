#EJERCICIOS TEMA 4


##	Ejercicio T4.1
    Buscar información sobre cuánto costaría en la actualidad un mainframe. 
    Comparar precio y potencia entre esa máquina y una granja web de unas prestaciones similares.

Si miramos la actualidad el más novedoso mainframe se lanzó el año pasado por IBM, he encontrado una pequeña 
comparativa con otros sistemas en la revista de IBM, 
(http://www.ibmsystemsmagmainframedigital.com/nxtbooks/ibmsystemsmag/mainframe_20160506/index.php#/14),
pero me resulta muy difícil realizar una comparación con una granja web con esas características pero es
evidente que una granja web resultara mucho más económica pero hay que tener en cuenta que también se precisa
de mucho más espacio para montarla y son costes que hay que determinar también.

![imagen](https://github.com/NiKaJim/SWAP/blob/ddc6480b98b05413febc1073e41ba554d7ded4a4/imagenes/ejerciciostema4/1.png)


##Ejercicio T4.2
Buscar información sobre precio y características de balanceadores hardware específicos.
Compara las prestaciones que ofrecen unos y otros.

Resulta muy difícil encontrar información sobre el precio, siempre recurren a formularios para solicitar presupuestos adaptados,
pero en el siguiente enlace si que se realiza una comparativa bastante extensa de algunos  balanceadores hardware.


https://kemptechnologies.com/es/server-load-balancing-appliances/product-matrix.html

![imagen](https://github.com/NiKaJim/SWAP/blob/ddc6480b98b05413febc1073e41ba554d7ded4a4/imagenes/ejerciciostema4/2.png)
 



##	Ejercicio T4.3
Buscar información sobre los métodos de balanceo que implementan los dispositivos recogidos en el ejercicio 4.2

Por ejemplo para el modelo LM2600:
https://kemptechnologies.com/es/server-load-balancing-appliances/loadmaster-2600/overview/

![imagen](https://github.com/NiKaJim/SWAP/blob/ddc6480b98b05413febc1073e41ba554d7ded4a4/imagenes/ejerciciostema4/3.png)
 

##	Ejercicio T4.4
Instala y configura en una máquina virtual el balanceador ZenLoadBalancer. 
Compara con la dificultad de la instalación y configuración usando nginx o haproxy (práctica 3).



## Ejercicio T4.5
 Probar las diferentes maneras de redirección HTTP. 
¿Cuál es adecuada y cuál no lo es para hacer balanceo de carga global? ¿Por qué?

El tipo de redirección indica si es temporal (301) o permanente (302).

Si queremos indicar a buscadores u otros visitantes de la página que una redirección es temporal utilizamos 302 y si queremos fijar la redirección de manera permanente utilizamos 301.
Para un usuario que se conecte a nuestra página le va a dar un poco igual que redirección utilices, porque el efecto será el mismo: que el navegador usuario se redirigirá a la dirección que hayamos indicado. 
La diferencia fundamental la captan los motores de búsqueda como Google, que con 302 entenderán que sólo se trata de un cambio en la URL de manera temporal y con 301 les estamos diciendo que actualicen la ruta de la página en sus bases de datos de manera definitiva.


## Ejercicio T4.6
   Buscar información sobre los bloques de IP para los distintos países o continentes.
   Implementar en JavaScript o PHP la detección de la zona desde donde se conecta un usuario.

Cada país tiene asignado un código ISO3166 así como un número preciso de cantidad de direcciones IP. 
Las podemos consultar directamente a través del siguiente enlace:
https://www.maxmind.com/es/allocation-of-ip-addresses-by-country

![imagen](https://github.com/NiKaJim/SWAP/blob/ddc6480b98b05413febc1073e41ba554d7ded4a4/imagenes/ejerciciostema4/4.png)

 

Para detectar la zona donde se conecta un usuario tenemos herramientas muy eficaces como http://iplocationtools.com/

Además desde http://chir.ag/projects/geoiploc/ podemos acceder al código en php para usarlo en nuestras aplicaciones.

![imagen](https://github.com/NiKaJim/SWAP/blob/ddc6480b98b05413febc1073e41ba554d7ded4a4/imagenes/ejerciciostema4/5.png)

 


##	Ejercicio T4.7
    Buscar información sobre métodos y herramientas para implementar GSLB.

    Mediante GSLB se realiza el balanceo de carga global, de forma que la carga se distribuye entre varios centros de datos.
    Se intenta minimizar los retrasos en las comunicaciones por las distancias entre el usuario y los servidores.
    Esto tiene la ventaja añadida de que si un centro falla, el tráfico se redirige a otro centro de datos (redundancia). 

    Hay varias formas de implementar el GSLB:

   - Uso del sistema de DNS
   - Redirección HTTP
   - GSLB basado en DNS
   - GSLB usando protocolos de enrutamiento

  A pesar de la alta disponibilidad que se obtiene usando GSLB, se trata de un sistema muy complejo de implementar,
  o por lo menos esto indican los apuntes de la asignatura …, ya que por ejemplo desde
  http://www.clm.com.pe/productos/a10/ax-global-server-load-balancing.htm ,nos indican que la implementación por DNS es “muy fácil” .

