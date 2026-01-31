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
    php artisan serve

2. Crear la API

abrir en el proyecto:
    routes/api.php

Al final del archivo, pegar:

use Illuminate\Http\Request;
use Illuminate\Support\Facades\Route;

use Illuminate\Support\Facades\Route;

Route::get('/hola', function () {
    return "Hola, esta es mi primera API en Laravel";
});

3. Probar la API en el navegador http://127.0.0.1:8000/api/hola

4. Cambia la ruta para provbarlo en POSTMAN:
    Route::get('/usuarios', function () {
        return [
            ["nombre" => "Juan"],
            ["nombre" => "Ana"]
        ];
    });

5. Probar la ruta en POSTMAN. Hacer un GET con la URL http://127.0.0.1:8000/api/usuarios.
