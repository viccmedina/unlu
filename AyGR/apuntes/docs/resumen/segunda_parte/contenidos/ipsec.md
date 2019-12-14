# IPSec

Conjutno de protocolos cuy función es asegurar la comunicación sobre IP, autenticando y / o cifrando 
los paquetes.

Actúa en capa de Red.

**Modo Transparente**, sólo la carga útil es cifrada o autenticada en el paquete IP. El ruteo no se ve 
afectado ya que la cabecera IP no es modificada ni cifrada. Puede suceder que cuando se emplea la 
cabecera de autenticación (AH) las direcciones IP no se puedan traducir.

**Modo Túnel**, todo pauqte IP es cifrado o autenticado. Para ello debe ser encapsulado en un nuevo 
paquete IP oara que pueda ser ruteado. Este modo es utilizado para comunicaciones de red a red.


## Protocolos Asociados

#### Authentication Header (AH)

Proporciona integridad, autenticación y no repudio si se leigen los algoritmos criptográficos adecuados.
No provee confidencialidad y asegura la carga del paquete IP y porciones del header.

#### Encapsulating Security Payload (ESP)

Proporciona confidencialidad y la opción de autenticación y protección de integridad. Asegura sólo la 
carga del paquete IP y no sus headers.