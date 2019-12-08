# Puentes Transparentes 

Los puentes transparenes se denominan así porque su presencia y operación son transparentes para los 
hosts de la red. Cuando se activan puentes transparentes, aprenden las ubicaciones de las estaciones
de trabajo analizando las direcciones de origen de las tramas entrantes de todas las redes conectadas.
Por ejemplo, si un puente ve una trama que llega del puerto 1 desde el host A, el puente concluye que el
host A puede ser alcanzado por el segmento conectado al puerto 1. A través de este proceso, los puentes
transparentes construyen una tabla (proceso de aprendizaje).

El puente utiliza una tabla como base para el reenvío de tráfico. Cuando se recibe una trama en una de
las interfaces del puente, este busca la dirección de destino de la trama en su tabla interna. Si la
tabla contien la asociación entre la dirección de destino y cualquier de los puertos del puente (aparte
de aquél en el que se recibió la trama), se remite la misma al puerto indicado. Si no se encuentra 
ninguna asociación, la trama se envía a todos los hosts (provocando inundación), excepto en el puerto
de entrada de dicha trama.

Los puentes transparentes aislan el tráfico con éxito, reduciendo así el tráfico visto en cada segmento
individual. Esto se denomina filtrado y ocurre cuando una dirección MAC de origen y destino residen en
la misma interface del puente.

### Definición de Puente como dispositivo

Dispositivo de interconexión de redes (o de división de segmentos) que opera en capa 2 (enlace).
Permite la conexión de redes sin la necesidad de un router.

Se diferencia del **Switch** por la cantidad de interfaces (un switch posee un número mayor).

Se diferencia del **Hub** dado que este realiza inundación únicamente. El **Puente** aisla dominios
de colisión, ya que reenvía tramas pertenecientes a cada segmento.
