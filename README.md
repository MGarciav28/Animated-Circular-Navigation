# CREANDO UN MENU DE NAVEGACIÓN CIRCULAR

Esta practica consiste en la creacion de un menú circular de navegacion compuesto por un botón principal, circular, centrado, el cual al ser presionado comienza una animacion de girar su icono y despliega desde el centro 8 nuevos botones que orbitan al principal en el sentido de las manecillas del reloj.

Cada icono de los botones secundarios cambia de color al pasar el mouse sobre el.

Al presionar nuevamente el boton principal se ocultan los botones secundarios orbitando en el sentido opuesto a las manecillas del reloj y terminando detras del boton principal, regresando a la posicion inicial.

## TECNOLOGÍAS
Esta práctica es realizada utilizando HTML, CSS, JAVASCRIPT. Se compone de un div con clase menu que funciona como contenedor para 9 elementos, los cuales son: un segundo div con clase toggle que funcionara como boton principal y 8 elementos li que conforman los enlaces. Cada uno de estos elementos contiene su correspondiente icono, obtenido de IONICONS.

El div contenedor sirve para centrar todos los iconos empleando flexbox.

El div toggle adquiere border-radius de 50% para tomar forma circular, se posiciona hasta el frente de todos los elementos con z-index y al ser presionado llama a la accion una funcion de javascript que añade o retira la clase "active" del div menú; junto a esta llamada se comienza la transformación de girar el div toggle 315 grados.

Los li se posicionan originalmente hasta el extremo izquierdo del contenedor con *left:0;*, artificialmente se mueven hacia la derecha con *transform-origin: 100px;*, y al cambiar la clase "active" del div menu