# Guía de instalación del TFG Shared Courses en WINDOWS
## Herramientas necesarias
- [XAMPP](https://www.apachefriends.org/es/index.html)
- [Visual Studio Code](https://code.visualstudio.com/)
- Cualquier navegador web

## Inicializar servidor usando XAMPP
Una vez XAMPP este instalado, se mostrará un panel como se muestra en la siguiente figura:
![Inicializar XAMPP](images/xampp_start.PNG)

Hay que inicializar los modulos de Apache y MySQL haciendo click en Start en la columna de Actions.

Luego hay que hacer click en admin a la derecha del boton Start de la fila del modulo de MySQL para inicializar phpMyAdmin.

## Crear base de datos con phpMyAdmin
Una vez abierto se muestra una interfaz como en la figura:
![phpMyAdmin Home](images/phpmyadmin_home.png)

Antes de todo, hay que hacer unos preparativos para subir el archivo de la base de datos:

Primero hay que cambiar el valor de max_allowed_packet ya que el archivo de la base de datos es más grande de lo que permite la configuración del servidor predeterminada, para ello hay que dirigirse a la pestaña SQL y ejecutar el siguiente comando (usando el boton de Continuar):

`SET GLOBAL max_allowed_packet = 67108864;`

Hay que crear la base de datos vacía antes de ejecutar el script .sql en ella, por tanto hacemos click en Nueva en el panel de la izquierda:

![new db](images/new_schema.png)

Luego nos muestra otra imagen donde podemos elegir la compatibilidad de carácteres de la base de datos, continuamos con la predeterminada y le damos a crear:

![new db](images/create_schema.png)

`SET GLOBAL event_scheduler = ON;`
[Descargar paquete de videos](https://drive.google.com/drive/folders/1SC_jgFkBqCy-ftMCoPK9tOlY6TVPv7xB?usp=sharing)
