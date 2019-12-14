# Security Shell (SSH)

Su uso más común es el logueo remoto. La información va de manera no legible. 

Puede hacer túneles para conexiones y transportar cualquier tipo de datos.

Se crean claves públicas y privadas, se les pasa la clave pública a los otros hosts y se establece una 
conexión SSH.

Se compone por:

``SSh Transport Layer``

Cufra y autentica. Provee autenticación, confidencialidad e intefridad.

``SSH Protocolo de Autentincación de Usuarios``

Para autenticar usuarios frente al servidor.

``SSH Protocolo de Conexión``

Abren canales de comunicación para intercambiar datos. Multiplexa distintos canales de comunicación 
lógicos.