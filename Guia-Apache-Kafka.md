# Guia - Kafka

## Componentes

### Kafka Broker

Es un servidor,y como tal escucha alguna conexión TCP por un puerto predeterminado de Kafka.

### Producer

Abstracción de productores: Producen contenido hacia el broker

### Consumer

Abstracción de consumidor: Consumen contenido del broker

### Conexión

Es de TCP y es una conexión TCP sin procesar, por lo que es bidireccional,permitiendo que el producer envie y reciba información del broker

### Topics

Particiones lógicas dentro del Broker donde se escribe contenido
(Son la cola de mensajes)

## Interacción

Producer establece una conexión TCP con el Broker,envia información
a un tópico específico.
La información es indexada y mantienen una posición en el tópico.

El Consumer consume la información,pero puede seleccionar. Kafka no es un modelo de empuje.

## Crecimiento de los tópicos

Se introducen las particiones dentro de los tópicos,estas particiones indican el intervalo de contenido que aceptan.(Ejemplo A-M y N-Z).

Cuando un Producer publica información,ahora debe saber en qué tópico y en que partición de este enviarla.Cuando lo hace,el Broker le devuelve la posición de esta información que se encuentra en el Broker.  

El Consumer también debe saber que partición de los tópicos consumir.  

## Queue vs Pub Sub

Queue : Mensaje publicado una vez,consumido una sola vez  
Pub Sub: Mensaje publicado una vez,consumido muchas veces  

Kafka es  
Consumer Group: Es una forma de agrupar o separar a los consumidores
para lograr uno de los dos métodos anteriores

Si agrupa a los consumidores,el sistema se convertirá en una cola correctamente. Un consumidor será responsable de una partición del tópico y esta no será vista por nadie.(No olvidar que no kafka no es un modelo de push,por lo que la información se sigue manteniendo pero será confirmada como leída).

Si cada consumidor tiene su grupo único,el sistema se convertirá en un pub-sub,permitiendo que una partición sea consumida por multiples Consumer. A la par nos ofrece procesamiento paralelo

***NO OLVIDAR : La particion es un derecho dependiente del grupo de consumidores.Si en un grupo un consumir se encarga de la partición 2,ningún otro del mismo grupo podrá encargarse de esta***

## Sistema distribuido Kafka

La replicación de particiones y tener una como líder de esta es posible en Kafka.

Un tópico no contiene una etiqueta líder y los demás una de seguidor,si no las particiones dentro de estos tendrán la etiqueta.
En un Topic 1,la partición 1 será el líder para todos los demás tópicos,pero dentro del Topic 2,la partición 2 es una seguidora de otra partición en otro tópico.

¿Quién gestiona estas etiquetas y datos? **ZOOKEEPER**

## Zookeeper

Por un sistema de chismes logra que las particiones seguidoras realicen copias actualizadas de la partición líder.Además de que maneja por este mismo sistema una comunicación para saber cual es la partición lider.