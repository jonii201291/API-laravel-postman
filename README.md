# API-laravel-postman
Una API es un conjunto de reglas, protocolos definiciones que permite que dos aplicaciones se comuniquen e intercambien datos entre sí.

Creación en Laravel y probada en Postman.

1. Preparación del Entorno

Instalar composer, PHP y POSTMAN.
En el terminal de VSC nos pondremos en la ruta donde se encuentran los archivos de XAMPP para crear el proyecto. En mi caso y para que sirva de orienteción, una vez situado en C://:
    cd xampp/htdocs
    
1. Crear el proyecto:
    composer create-project laravel/laravel nombreProyecto

Acceso al proyecto:
    cd nombreProyecto

Arrancar el servidor(la URL será  127.0.0.1:8000):
    cd .
    php artisan serve

2. Crear la ruta para mostrarlo en el navegador:
    En el archivo routes/web.php
   <img width="508" height="98" alt="image" src="https://github.com/user-attachments/assets/e5cfeae1-a070-4a0b-ad55-1b0b22e8805b" />

    En el navegador http://127.0.0.1:8000

3.  Crear la API
    En el archivo routes/api.php

    <img width="618" height="170" alt="image" src="https://github.com/user-        attachments/assets/a3e60036-dd91-4528-a12b-6d40904d8a32" />

    En el navegador http://127.0.0.1:8000/api/hola
