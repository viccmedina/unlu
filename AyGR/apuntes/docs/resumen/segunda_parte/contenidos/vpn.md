# Redes Privadas Virtuales (VPN)

Construir un camino seguro sobre un medio inseguro.

Conjunto de herramientas que permiten a redes de diferentes lugares conectar de forma segura, 
utilizando una red pública como capa de transporte.

Utiliza cifrado para proveer confidencialidad, autenticidad e integridad.

### Objetivos

* Conectar de forma segura dos redes empresariales.
* Vincular sucursales con una red empresarial.
* Poder conectar socios, proveedores, clientes a la red de la organización.

### Servicios

``Autenticación de Usuarios``

Solamente usuarios autorizados pueden tener acceso a la VPN.

``Administración de Claves``

Se pueden generar y actualizar las claves de cifrado para los clientes VPN y el servidor VPN.

``Administración de Direcciones``

Se deben asignar a los clientes VPN las direcciones IP dentro de la red corporativa y asegurar que 
dichas direcciones se mantengan privadas.

``Cifrado de Datos``

Los datos transportados sobre la infraestructura de la red pública tienen que ser ilegibles para los 
clientes no autorizados de la VPN.

``Encapsulamiento``

La tecnología VPN debe encapsular los datos privados agregando una cabecera adicional que permita a 
estos transitar por la red pública, a esto se lo conoce como túnel.

``Soporte de Múltiples Protocolos``

Proveer soporte para los protocolos utilizados en la red pública.


### Tipos

``De Acceso Remoto``

Conectan usuarios a través de un servidor de Acceso de Red (NAS). Interactúan con server de 
autenticación, autorización y contabilidad.

``Site to Site``

Conectan redes con redes mediante gestores de tráfico.