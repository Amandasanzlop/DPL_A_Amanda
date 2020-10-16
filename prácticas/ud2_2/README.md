# DPL_A_Amanda

Para instalar Apache, en primer lugar, actualizamos el índice de paquetes locales para que reflejen los últimos cambios anteriores:

![Captura1](1.png)


Instalamos Apache haciendo uso de "sudo apt install apache2":

![Captura2](2.png)


Antes de probar Apache, es necesario modificar los ajustes de firewall para permitir el acceso externo a los puertos web predeterminados.
Durante la instalación, Apache se registra con UFW para proporcionar algunos perfiles de aplicación que pueden utilizarse para habilitar 
o deshabilitar el acceso a Apache a través del firewall. Enumeramos los perfiles ufw y habilitamos el perfil Apache, que es el más restrictivo.
En esta ocasión, sólo vamos a permitir el tráfico en el puerto 80:

![Captura3](3.png)


Verificamos el cambio. Obtenemos como respuesta que el firewall no está activo. Para solucionarlo, activamos el firewall.

![Captura4](4.png)


Realizamos una verificación con el sistema init systemd para saber si se encuentra en ejecución el servicio:

![Captura5](5.png)


Otra forma de comprobar que el servidor web está funcionando, es solicitar una página de Apache. Es decir, 
podemos acceder a la página de destino predeterminada de Apache para confirmar que el software funcione correctamente mediante su dirección ip.

![Captura6](6.png)


Detenemos el servidor web:

![Captura7](7.png)


Iniciamos el servidor web cuando no está activo:

![Captura8](8.png)


Detenemos y luego iniciamos el servicio de nuevo:

![Captura9](9.png)


Si solo realiza cambios de configuración, Apache a menudo puede recargarse sin cerrar conexiones. Para hacerlo:

![Captura10](10.png)


Por defecto, Apache está configurado para iniciarse automáticamente cuando el servidor (Ubuntu) lo hace. Si no es lo que se quiere, deshabilitamos este
comportamiento:

![Captura11](11.png)


Para volver a habilitar el servicio de modo que se cargue en el inicio:

![Captura12](12.png)








