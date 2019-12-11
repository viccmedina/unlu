# Sistema de Detección de Intrusos (IPS)

Un **IDS** monitorea y busca identificar patrones que puedan indicar un ataque o violación a una 
política de seguridad, ya sea de red o a sistemas en particulares.

Puede basarse en firmas, patrones y / o herurísticas del tráfico monitoreado.
Un IDS identifica ataques una vez que éstos están en proceso, o que ya ocurrieron (``NO previenen``).

Pueden generar alertas e interactuar con Firewalls para contener un ataque en proceso.


# Sistema de Prevención de Intrusos (IPS)

Se denomina **IPS** a los dispositivos de red especializados que al igual que los IDS monitorean el 
tráfico tratando de identificar posibles ataques, pero actúan "en el medio" y activamente intentan 
prevenir o bloquear dichos ataques.

Operan utilizando análisis estadístico.

Posibles acciones:

- Generar alarmas
- Descartar paquetes
- Resetear conexiones TCP
- Bloquear tráfico basa en direcciones IP.

Pueden considerarse un tipo de Firewall.