# Watson-Assistant - Virtual-Agent

Watson assistant es un bot cognitivo que puede ser personalizado para adaptase a sus necesidades empresariales, el asistente direcciona las consultas de sus clientes a un conocimiento, lo que proporciona la respuesta adecuada. Los conocimientos de diálogo devuelven respuestas que son creadas por el usuario para proporcionar información sobre los temas o tareas sobre los que los usuarios realizan preguntas y sobre cómo preguntan sobre las mismas y el producto crea de forma dinámica un modelo de aprendizaje automático que se adapta para comprender las mismas solicitudes de usuario y otras similares.

Watson assistant es un bot alojado completamente que está gestionado por IBM Cloud, lo que significa que no tiene que preocuparse por configurar o mantener la infraestructura para darle soporte.

## 1. Conceptos Básicos 📋 
### Dialog skill
Una Skill es un contenedor para la inteligencia artificial que le permite a un asistente ayudar a sus clientes.

Un asistente dirige las solicitudes por el camino óptimo para resolver un problema del cliente. Agregue habilidades para que su asistente pueda proporcionar una respuesta directa a una pregunta común o hacer referencia a resultados de búsqueda más generalizados para algo más complejo
Un dialog skill comprende las preguntas o solicitudes típicas de los usuarios y las responde o las cumple siguiendo un diálogo escrito por usted.

### Itens
Una intención representa el propósito de la entrada de un usuario, como una pregunta sobre ubicaciones de negocios o un pago de facturas. Usted define una intención para cada tipo de solicitud de usuario que desea que su aplicación admita. El nombre de una intención siempre tiene el prefijo del caracter ``` #```. Para entrenar la habilidad de diálogo para reconocer sus intenciones, usted proporciona muchos ejemplos de entrada del usuario e indica a qué intenciones se asignan.

Se proporciona un catálogo de contenido que contiene intenciones comunes preconstruidas que puede agregar a su aplicación en lugar de crear la suya propia. Por ejemplo, la mayoría de las aplicaciones requieren una intención de saludo que inicia un diálogo con el usuario. Puede agregar el catálogo de contenido General para agregar una intención que salude al usuario y haga otras cosas útiles, como finalizar la conversación.

### Dialogo
Un diálogo es un flujo de conversación ramificado que define cómo responde su aplicación cuando reconoce las intenciones y entidades definidas. Utiliza el editor de diálogo para crear conversaciones con los usuarios, proporcionando respuestas basadas en las intenciones y entidades que reconoces en su entrada.

Para permitir que su habilidad de diálogo maneje preguntas más matizadas, defina entidades y haga referencia a ellas desde su diálogo.

### Entidades
Una entidad representa un término u objeto que es relevante para sus intentos y que proporciona un contexto específico para un intento. Por ejemplo, una entidad podría representar una ciudad donde el usuario desea encontrar una ubicación comercial o el monto de un pago de facturas. El nombre de una entidad siempre tiene como prefijo el caracter ```@```.

Puede entrenar el dialog skill para reconocer sus entidades proporcionando valores y sinónimos de términos de entidad, patrones de entidad o identificando el contexto en el que una entidad se usa típicamente en una oración. Para ajustar su diálogo, regrese y agregue nodos que verifiquen las menciones de la entidad en la entrada del usuario además de las intenciones.

Mas información en: 
https://cloud.ibm.com/docs/assistant?topic=assistant-skills
https://cloud.ibm.com/docs/services/assistant-icp?topic=assistant-private-getting-started

## 2.Desarrollo de un Watson Assistant por medio de IBM CLOUD 🚀

 es algo que siempre debes tener en cuenta cuando piensas en cómo proporcionar la mejor experiencia conversacional

_Estas instrucciones te permitirán obtener un WatsonAssitent funcional._

```
Da un ejemplo
```


## 3. Conservar el Watson Assistant 🔧

Para que tu WatsonAssisten se mantenga siendo funcional es recomendable:

### 2.1 Actualiza los intentes:
Siempre que sea posible crear nuevas entidades o elimina las que los usuarios realmente no esten utilizando.
### 2.2 Escribe diferentas formas de un mismo mensaje:
Los usuarios pueden preguntar de diferentes formas es por eso que es necesario que una sola pregunta tenga varias versiones.
### 2.3 Guía a los usuarios a través de la conversación:
Para que los usuarios tengan una buena experencia y deseen seguir usando en assistant es necesario que se guien desde el principio hasta el final de la conversación.
### 2.4 Cuida el flujo de la conversación:
Cada interación deben conducir a la siguiente que ya fue definida. Es conveniente que la conversación este guionizada para que los usuarios solo tengan que seguir el guion creado.
### 2.5 Asegurece que su interfaz conversación este siempre actualizada:
watson assistant esta diseñado para simular una conversación, pero se recomienda no solo usar textos sino que por medio de IBM también se puede enriquecer con imágenes, botones, etc.


## Construido con 🛠️
_Se uso IBM Cloud para utilizar el servicios de watson-assisten que nos proporciono las herramientas necesarias para crear el chat-bot_
* [IBM](https://www.ibm.com/cloud/watson-assistant/) - El servicio


## Mas información 📖
Puede hacer uso de esto u otros servicios en la nube  [IBM-CLOUD](https://www.ibm.com/co-es/cloud)


## Autores ✒️
* **IBM** - *Equipo IBM Cloud*



---
