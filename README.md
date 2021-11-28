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
&nbsp;<img src="./Imagenes/3_3.png" width="374">&nbsp;<img src="./Imagenes/3_4.png" width="350">
