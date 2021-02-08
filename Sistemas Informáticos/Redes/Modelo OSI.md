# Modelo OSI
Es un modelo conceptual que caracteriza y estandariza las funciones de comuncinación de un sistema informático o de telecomunicaciones sin tener en cuenta su estructura y tecnología internas subyacentes. Su objetivo es la interoperabilidad de divrsos sistemas de comunicación con protocolos de comunicación estándar.

## Capas
### Física
Se encarga de enviar los datos por el medio de transmisión. En este nivel se definen las características eléctricas y mecánicas de la red que son necesarias para establecer y mantener la conexión física.

### Enlace de datos
Se encarga de establecer y mantener el flujo de datos que discurre entre los usuarios. Controla si se van a producir errores y los corrige.

### Red
Se encarga de decidir por dónde se transmitirán los datos en el interior de la red. Permite que los datos sean enviados de una red a otra por medio de los enrutadores.

### Transporte
Garantiza que los datos se envían de manera fiable desde el nodo de transmisión hacia el nodo de destino, tambien asegura la transferencia de información a pesar de los fallos que pudieran ocurrir en los niveles anteriores.

### Sesión
Permite que dos aplicaciones en diferentes computadoras establezcan, usens y terminen la conexión llamada sesión. El nivel de sesión define el diálogo que se requiere en la comunicación de los dispositivos.

### Presentación
Se encarga de formatear los datos. Cada tipo de red utiliza un esquema de formato particular que se aplica en la capa de presentación. La capa de presentación garantiza que los números y el texto se envían para que puedan ser leídos por la capa de presentación del nodo de recepción.

### Aplicación
Se encarga del intercambio de información entre los usuarios y el sistema operativo. Representa los accesos a las aplicaciones y a los servicios de red de los usuarios de una computadora.