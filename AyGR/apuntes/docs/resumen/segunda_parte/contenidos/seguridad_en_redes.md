# Seguridad en Redes

### Arquitectura de la Seguridad

``Ataque a la Seguridad``

Cualquier acción que comprometa a la seguridad e la información perteneciente a una organización.

``Mecanismos de Seguridad``

Un proceso (o dispositivo que incorpora dicho proceso) que tiene por objetivo detectar, prevenir o 
restaurar un ataque a la seguridad.
Por ejemplo cifrado, firma digital, control de acceso, control de tráfico, etc.

``Servicios de la Seguridad``

Un proceso o servicio de la comunicación que realza la seguridad de los sistemas de procesamiento de 
datos y de las transferencias de información de una organizaciń. Los servicios buscan contrarrestrar 
los ataques de seguridad, y pueden valerse de uno o más mecanismos de seguridad para proveerlo.


### Servicios de Seguridad

``Confidencialidad``

La información que circula por la red sólo puede ser leída por las partes autorizadas.

``Autenticación``

Asegura la identidad del emisor, y que esta no sea falsa.

``Intgridad``

La información debe llegar a destino sin modificaciones.

``Disponibilidad``

Los recursos deben estar disponibles para las partes autorizadas.

``Control de Acceso``

Determinar que recursos son accedidos por cada grupo de usuarios.

``No Repudio``

El emisor / receptor de un mensaje no pueden negar la recepción del mismo.


### Impacto Potencial

``Bajo``

Ante la pérdida de confidencialidad, integridad o disponibilidad puede esperarse que tenga un impacto 
limitao en las operaciones, recursos o individuos de la organización.

``Moderado``

Ante la pérdida de confidencialidad, integridad o disponibilidad puede esperarse que tenga un impacto 
serio en las operaciones, recursos o individuos de la organización

``Alto``

Ante la pérdida de confidencialidad, integridad o disponibilidad puede esperarse que tenga un impacto 
catastrófico en las operaciones, recursos o individuos de la organización.


### Ataques

``Interrupción``

La información nunca llegará a destino. Afecta a la **Disponibilidad**.

``Intercepción``

El destino recibe la información enviada desde por el origen, pero éste ha sido interceptada por un 
tercero. Afecta a la **Confidencialidad**

``Generación``

El intruso genera y envía la información al destino, haciendose pasar por el origen real. Afecta a la 
**Autenticación**.

``Modificación``

La información enviada por el origen es interceptada por el atacante, modificada y reenviada al 
destino. Afecta a la **Integridad***


### Intrusos

``Pasivos`` 

Es aquél que accede a los recursos e información que se suponen que son confidenciales, sin realizar 
ninguna acción sobre ellos, es decir, visualiza los datos o monitoriza tráfico de red.

``Activos``

Es aquél que modifica archivos, BD o reenvía información que es capaz de capturar. Es capaz de generar 
nuvos datos / mensajes

### Seguridad por

``Profundidad``

Implementar mecanismos de seguridad a distintos niveles: hardware, software, mantenimiento, 
actualización, etc.

``Diseño``

Desde la concepción de un sistema debe tenerse en cuenta la seguridad.

``Transparencia``

Evitar basarse en secretos, utilizando algoritmos y mecanismos bien evaluados.

### Políticas de Seguridad

