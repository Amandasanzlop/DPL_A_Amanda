# DPL_A_Amanda

Para cada máquina, la configuración del adaptador red en el Virtualbox sería:

![Captura1](1.png)

![Captura2](2.png)


Se realiza la configuración IP en Windows 7:

![Captura3](3.png)


Se configura el nombre del equipo y se añade a un grupo de trabajo que se llama DESPLIEGUEXX:

![Captura4](4.png)


Se configura el adaptador de red en Ubuntu Server. Se averigua el nombre que el sistema ha asignado a nuestra interfaz, utilizando el comando ifconfig:

![Captura5](5.png)


Se edita el fichero de configuración de las interfaces de red:

![Captura6](6.png)


En Ubuntu ha sido necesario utilizar Netplan para configurar la red:

![Captura7](7.png)


En Windows 7 ha sido necesario crear una regla en Firewall:

![Captura9](9.png)


Comprobación de la configuración y de funcionamiento:

![Captura8](8.png)

![Captura10](10.png)















