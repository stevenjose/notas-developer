## Yii2

## Iniciar el servidor

```
php yii serve --port=8888

```

## Estructura de la aplicacion
```
basic/                  base path de la aplicación
    composer.json       archivo utilizado por Composer, describe información de sus paquetes y librerías
    config/             contiene la configuración de las aplicaciones (y otras)
        console.php     configuración de la aplicación de consola
        web.php         configuración de la aplicación web
    commands/           contiene las clases de comandos de consola
    controllers/        contiene las clases de los controladores
    models/             contienes las clases del modelo
    runtime/            contiene archivos generados por Yii en tiempo de ejecución, como archivos de log y cache
    vendor/             contiene los paquetes y librerías instalados por Composer, incluyendo el propio núcleo de Yii
    views/              contiene los archivos de vistas (templates)
    web/                raíz web de la aplicación, contiene los archivos accesibles vía Web
        assets/         contiene los assets publicados (javascript y css) por Yii
        index.php       el script de entrada (o bootstrap) de la aplicación
    yii                 el script de ejecución de los comandos de consola de Yii
```

### Llamar a una vista 

El metodo render recibe dos argumentos el nombre de la vista, y un array con las variables que se le quieren pasar a la vista. 

```
$this->render('nombre de la vista', ['message' => $message])
```