# Build Your Own IoT Platform 
## Building the Critical Components

### Creación de una base de datos principal de series temporales

- Creación de la base de datos en phpMyAdmin<br />
&nbsp;<img src="./Imagenes/1_1.png" width="350">
- Creación de un usuario para administrar las base de datos<br />
&nbsp;<img src="./Imagenes/1_2.png" width="300">
- Creación de una tabla de datos, con el esquema diseñado<br />
&nbsp;<img src="./Imagenes/1_3.png" width="500">

### Instalación de nodos requeridos en Node-RED

- Agregar el nodo MySQL a la paleta Node-RED<br />
&nbsp;<img src="./Imagenes/2_1.png" width="350">
- Nodo Mysql agregado<br/>
&nbsp;<img src="./Imagenes/2_2.png" width="100">

### Creación del primer flujo para la plataforma

- La primera secuencia de flujo en Node-RED con un inject node y debug node<br />
&nbsp;<img src="./Imagenes/3_1.png" width="325">&nbsp;<img src="./Imagenes/3_2.png" width="350">

#### Añadir la capacidad de publicación de MQTT

- Agregar un mqtt out node y configurar el mqtt broker<br />
&nbsp;<img src="./Imagenes/3_3.png" width="374">&nbsp;<img src="./Imagenes/3_4.png" width="350"><br/>
&nbsp; Vista del flujo con la capacidad de publicación mqtt<br />
&nbsp;<img src="./Imagenes/3_5.png" width="420">

### Publicador de mensajes de API REST
- Configuración de un http input node <br/>
&nbsp;<img src="./Imagenes/4_1.png" width="350">
- Configuración de los nodos de creación de mensaje y creación de respuesta <br/>
&nbsp;<img src="./Imagenes/4_2.png" height="270">&nbsp;<img src="./Imagenes/4_3.png" height="270">
- Vista del flujo de la API de publicación de mensajes<br/>
&nbsp;<img src="./Imagenes/4_4.png" height="230">
### Creación de un Database Listener
- Configuración del nodo mqtt input<br/>
&nbsp;<img src="./Imagenes/5_1.png" width="300">
- Configuración del nodo función para la creación de querys <br/>
&nbsp;<img src="./Imagenes/5_2.png" width="350">
- Inclusión y configuración del nodo MySQL usando la base de datos para time-series creado anteriormente.
&nbsp;<img src="./Imagenes/5_4.png" height="250">&nbsp;<img src="./Imagenes/5_3.png" height="250"> 
- Vista del flujo con el nodo MySQL y Database Listener<br/>
&nbsp;<img src="./Imagenes/5_5.png" width="450">


### REST API Message Retriever
- Configuración de los nodos http input<br/>
&nbsp;<img src="./Imagenes/6_1.png" height="250">&nbsp;<img src="./Imagenes/6_2.png" height="250">
- Configuración del function node para la creación de querys<br/>
&nbsp;<img src="./Imagenes/6_3.png" width="350"> 
- Flujo con la recuperación de mensajes del almacenamiento <br/>
&nbsp;<img src="./Imagenes/6_4.png" width="450"> 

### Verificar que todo funcione como se esperaba
- Verificación de la base de datos, <br/>
&nbsp;<img src="./Imagenes/7_0.png" width="450"> 
- Verificación del primer flujo <br/>
&nbsp;<img src="./Imagenes/7_1.png" width="450"> 
- Verificación del segundo flujo flujo <br/>
&nbsp;<img src="./Imagenes/7_2.png" width="450"> 
- Verificación del tercer flujo flujo <br/>
&nbsp;<img src="./Imagenes/7_3.png" width="450">
- Verificación del cuarto flujo <br/>
&nbsp;<img src="./Imagenes/7_3.png" width="450"> 
### Ejecutar Node-RED en segundo plano de forma continua
- En este caso se usa docker para la ejecución en segundo plano y el despliegue automático. <br/>
&nbsp;<img src="./Imagenes/8.png" width="450"> 
