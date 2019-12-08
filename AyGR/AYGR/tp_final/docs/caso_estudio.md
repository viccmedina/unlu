# Caso de Estudio: "Sistema de Peajes - Autopista del Norte"

Se requiere el diseño de red de telecomunicaciones para suplir las necesidades de la empresa "Autopista del Norte S.A": La misma cuenta con:

* Una casa central en CABA.
* Una estación en "San Vicente" con cuatro cabinas.
* Una estación en "Las Heras" con cuatro cabinas.
* Una estación en el Corredor Norte (entre la ruta 8 y 9) con seis cabinas.

# Estación de Peaje
Cada estación de peaje cuenta, además de las cabinas de cobro, una oficina de gestión. Las estaciones de pejaes deberán estar comunicadas entre sí y con la Casa Central mediante una red privada, sin acceso a Internet.

Las estaciones de pejae deberán contar con telefonía interna entre las cabinas de una misma estación, la oficina de administración correspondiente, y la Casa Central. Es requisito importante que se brinde una buena calidad en la comunicación por voz.

Además de telefonía y datos de facturación, la red de comunicaciones deberá dar soporte de flujo de video proveniente de cámaras IP instaladas en cada estación. Por razones de confidencialidad y privacidad, los únicos autorizados para acceder a estos flujos de video son las oficinas de gestión de cada estación.

# Casa Central
La casa central sí provee servicios hacia Internet: la consulta de saldos del sistema de telepeajes, la carga virtual, y un sistema para registrar "usuarios vecinos" a los cuales se les cobrará una tasa diferencial. Estos servicios deberán operar sobre la web utilizando mecanismos de seguridad estándares. 

Toda la información se almacena en una base de datos centralizada. La casa central provee, además, un servicio de alerta vía correo electrónico para casos de congestión y para el envío de información relevante a sus usuarios registrados.

Entre la red pública de Internet y la red privada deberá implementarse un cortafuegos que denegue todo tráfico excepto:

* el acceso desde Internet a los servidores expuestos en el párrafo previo,
* la conectividad en forma remota a los sistemas internos por parte de tres computadoras portátiles
  que son utilizadas por la gerencia general.

# Gerencia

Finalmente se debe contemplar que, en casos extremos, las estaciones de peaje pueden operar de forma independiente, aún con interrupciones en los servicios de energía eléctrica y conectividad hacia la Casa Central.

Tenga en cuenta que, de acuerdo a estimaciones oficiales, el corredor vial tiene un flujo estimado en casi 50 mil vehículos por día, siendo la mayoría camiones y transporte de carga.