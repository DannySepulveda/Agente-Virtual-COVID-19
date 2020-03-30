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

### Caso de uso 

Actualmente a nivel internacional se está presentando una pandemia ocasionada por el COVID-19, lo cual ha generado que las personas tengan muchas inquietudes las cuales no pueden aclarar tan fácilmente o de fuentes oficiales. Por esa razón se desarrolló un ChatBot con el fin de aclarar dichas dudas brindando información oficial con el fin de evitar que se cree pánico y desinformación. 

### Paso a paso del desarrollo 

### Paso 1:

Iniciar sesión en IBM Cloud, en caso de que no se cuente con una cuenta, crearla en este enlace https://cloud.ibm.com/registration

### Paso 2:

En la sección de catálogo buscamos Watson Assistant y se selecciona dicho servicio 

![1](https://user-images.githubusercontent.com/44415995/77944254-3d6ca000-7284-11ea-8760-ffb4c6dc5682.jpg)

### Paso 3:

Para crear el servicio de Watson Assistant, primero se debe seleccionar la región, en este caso se seleccionó Dallas y posteriormente selecciona el tipo de plan que más se acomode a sus necesidades. Una vez realizado esto se le asigna un nombre al servicio y se le da click a la opción de “Create” o “Crear”.

![2](https://user-images.githubusercontent.com/44415995/77944449-a05e3700-7284-11ea-86d0-e6d81c49dc90.jpg)

### Paso 4:

En la ventana que se cargó se le da click a “Launch Watson Assistant” o “Iniciar Launch Watson Assistant” y se abrirá una nueva ventana.

![3](https://user-images.githubusercontent.com/44415995/77944487-b1a74380-7284-11ea-867e-8de6afa46216.jpg)

### Paso 5:

Ahora se selecciona la opción de “Skill” la cual tiene este icono ![Icono1](https://user-images.githubusercontent.com/44415995/77944907-5c1f6680-7285-11ea-9ec6-8ebc41320025.jpg) y se selecciona “Create Skill” o “Crear skill”, luego se selecciona “Dialog Skill” y “Next” o “Siguiente”.

![4](https://user-images.githubusercontent.com/44415995/77944530-be2b9c00-7284-11ea-9ce7-145f3eb13d55.jpg)

### Paso 6:

Ahora se procede a configurar el modelo donde es importante asignarle un nombre y el idioma en el que se va a implementar el chatbot en este caso español.

![5](https://user-images.githubusercontent.com/44415995/77944551-c5eb4080-7284-11ea-9333-79afde5f6fb7.jpg)

### Paso 7:

El siguiente paso a seguir es entrenar el modelo, primero se comienza con los “intent” o “intenciones”, este entrena al asistente para comprender la variedad de formas en que los usuarios expresan una idea o inquietud. Para ello se selecciona “Create intent” y se le asigna un nombre a la intención y los ejemplos para entrenar el modelo.

![6](https://user-images.githubusercontent.com/44415995/77944644-eb784a00-7284-11ea-9ebf-da5e6f6b287e.jpg)

Por ejemplo el “Intent” de “Aislamiento_preventivo”, donde algunos de los ejemplos utilizados para entrenarlos fueron “¿Qué debe hacer la gente en casa cuando está en aislamiento?, como disminuir la probabilidad de adquirir la enfermedad?, que debo hacer en mi casa para que no me de COVID19”. Hay que tener en cuenta que entre más ejemplos se utilicen por “Intent” para entrenar el modelo, este será más preciso.

![7](https://user-images.githubusercontent.com/44415995/77944671-f9c66600-7284-11ea-92f4-90442d08e146.jpg)

### Paso 8:

Una vez ingresados los “Entity”, se ingresan las entidades los cuales son sustantivos o palabras clave, para ello se selecciona “Create entity” donde se le asigna un nombre y los sustantivos. Para este modelo se añadieron departamentos y municipios.

![8](https://user-images.githubusercontent.com/44415995/77944691-034fce00-7285-11ea-9694-72aa926c6822.jpg)

![9](https://user-images.githubusercontent.com/44415995/77944721-0fd42680-7285-11ea-9c79-dc0049b13377.jpg)

### Paso 9:

Ahora se procede a añadir los diálogos, para ello se debe seleccionar “Add node” o “Añadir nodo”. Posteriormente se le proporciona un nombre y selecciona ya sea un “Intent” o un “Entity” de los que fueron añadidos anteriormente y por último se procede a añadir el dialogo. 

![10](https://user-images.githubusercontent.com/44415995/77944806-31351280-7285-11ea-805a-a3d361b6be75.jpg)

## Nota: Para este chatbot los diálogos se desligan del nodo principal “Preguntas para resolver” por lo que se añadieron “Child node” a partir de ese nodo, al dar click en los 3 puntos.##

![11](https://user-images.githubusercontent.com/44415995/77944837-3eea9800-7285-11ea-9933-8523e71b3365.jpg)

Al momento de ingresar el dialogo en la parte inferior en el apartado de “Then assistant should”. Se selecciona “Jump to” y el nodo principal, en este caso “Mas opciones”

![12](https://user-images.githubusercontent.com/44415995/77944868-47db6980-7285-11ea-97db-cfad5e21959e.jpg)

### Paso 10:

El modelo se entrena automáticamente, una vez finalizado este proceso lo puede probar dando click en “Try it” con el siguiente icono ![Icono2](https://user-images.githubusercontent.com/44415995/77944935-65a8ce80-7285-11ea-9d3d-e91035e40b7b.jpg)

![13](https://user-images.githubusercontent.com/44415995/77944892-50cc3b00-7285-11ea-8c76-4ddcc5f151c6.jpg)

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

Es posible incorporar el Watson Assitant en un portal web [Incorporación](https://github.com/emeloibmco/Agente-Virtual-COVID-19/blob/master/Incorporaci%C3%B3nAssistant.md)


## Autores ✒️
* **IBM** - *Equipo IBM Cloud*



---
