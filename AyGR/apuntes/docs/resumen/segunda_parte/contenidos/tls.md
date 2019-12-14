# Transport Layer Security Protocol

Protocolos que proporcionan comunicaciones seguras por un red, comunmente Internet.

Se establece una conexión segura por medio de un canal cifrado entre el cliente y el servidor. Le 
brinda seguridad a TCP sin modificarlo.

Provee cifrado y autenticación X.509 de uno o ambos extremos.

Está formado por cuatro protocolos:

- **TLS Recod Protocol**, encargado de cifrar y enviar los mensajes. Toma un mensaje de capa superior, 
lo fragmenta en bloques, opcionalmente comprima cada bloque, aplica un código de autenticación y luego 
cifra el mensaje utilizando una clave privada y agrega el encabezado.

- **Handshake Protocol**, negocia la sesión TLS de una sesión TCP identificada con un número. Consta de cutro fases:
	- *Fase I*, el cliente envía un mensaje HELLO especificando parámetros como cifrado, compresión y 
		versión del protocolo SSL más alta permitida. Además se incluye el identificador de la sesión. 
		El server responde con un mensaje HELLO con los parámetros seleccionados que fueron ofertados 
		por el cliente.

	- *Fase II*, cuando los parámetros de la conexión son conocidos, cliente y servidor intercambian 
		certificados X.509.

	- *Fase III*, cliente y servidor negocian una clave secreta, que es descifrada con la clave pública 
		de cada uno.

	- *Fase IV*, se da por finalizada la sesión.

- **Alert Protocol**, mensaje de dos bytes para mandar alertas. El primer byte indica si es un warning 
o un fatal (en ese caso se da por finalizada la sesión). El segundo byte indica la alerta especificada.

- **Chance Chiper**, mensaje de un solo byte que indica que desde ahora se va a comenzar a utilizar 
todos los protocolos que se negociaron. Durante el handshake no se utiliza ningún cifrado, ya que el 
mismo se esta negociando.