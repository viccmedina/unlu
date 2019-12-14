# Funciones Hash

Una función hash es una función computable que aplicada a un mensaje "m" de tamaño variable genera una 
representación de tamaño fijo del propio mensaje H(m). H(m) es mucho menor que "m"

### Autenticación de mensajes

Procedimiento para verificar que el mensaje recibido ha sido generado por la supuesta fuente que lo 
envía, y que no ha sido modificado. Adicionalmente puede verificarse la secuencia y tiempo oportuno (
que no ha ocurrido una alteración en el orden de los mensajes, retrasos o retransnmisiones).


### Código de autenticación de mensajes

Una función MAC es una función aplicada a un mensaje "m" de tamaño variable y con una clave "K" que 
genera una representación de tamaño fijo del propio mensaje MAC=cK(m).
La clave secreta es compartida por el emisor y el receptor.