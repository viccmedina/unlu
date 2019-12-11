# Firewalls

Un firewall es un medio que sirve para regular el tráfico entre redes. Por ejemplo tráfico entrante y 
tráfico saliente de una computadora de la organización e Internet.

La información mínima que tiene un firewall de un paquete IP es la direcciío IP de origen y destino, 
más el puerto de origen y destino junto con el protocolo utilizado (TCP / UDP).

Permite o no, la comunicación de acuerdo a una política de seguridad que ha sido configurada 
previamente por un administrador. Implementadas mediante **Listas de Control de Acceso**, las cuales 
tienen la siguiente lógica:
	- Si el paquete viene de la red X, dejarlo pasar.
	- Si el paquete viene de la red Y, no dejarlo pasar.

### Servicios Estandares de los Firewalls

``Control de Acceso``

Obtiene tanta información como sea posible de los paquetes que pasan por él y de acuerdo a esa 
información y a la política de seguridad (que se ha definido), el paquete será o no autorizado. 

``Registro de Actividades``

Registra todas las actividades, autorizadas y denegadas, que lo atraviesan. Es una herramienta para 
supervisar la actividad de la red y detectar tráfico poco usual.


### Tipos de Firewalls

``Network Firewall``

- **Sin Estado**, filtrado de pquetes, basados en características de ese mismo paquete. Por ejemplo 
direcciones IP, puertos, etc. Podría decirse que opera en capa 3 y 4 (red y transporte).

- **Con Estado**: filtrado de paquetes basados en características de ese mismo paquete junto con el 
estado actual de la conexión TCP / UDP.

``Application Firewall``

- **De Red**, lo más comunes son los proxies o los waf (web application firewall) que trabajan a 
nivel de HTTP. Filtran en la capa de aplicación, generalmente por usuario o por sesión.

- **De Host**,  monitorea las llamas al sistema operativo de un proceso, bloqueando aquellas que 
estan fuera del patrón común de uso, o fuera de la política de seguridad definida para éste.


Independientemente del tipo de Firewall, en todos los casos se analiza y en base a la política de 
seguridad cnfigurada, se realiza una acción: bloquear, rechazar, permitir, registrar, alertar, etc el 
paquete, tráfico o evento de red.