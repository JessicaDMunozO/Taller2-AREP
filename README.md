# Taller 2 - AREP
Para este taller se trabajó sobre un servidor web en Java que debe retornar los archivos solicitados del disco local. En particular se tienen archivos *html*, *java script*, *css* e imágenes.
Los cuales se relacionan con el tema de películas trabajado en el taller anterior.
## Empezando
Las siguientes instrucciones permiten que obtenga una copia del proyecto en funcionamiento.
### Prerrequisitos
1. Debe contar con un IDE (entorno de desarrollo integrado) para facilitar la ejecución del código.
2. Debe tener Maven y JDK para compilar y ejecutar el proyecto.
3. Verificar que el puerto 35000 esté disponible para que el servidor web lo pueda usar sin inconvenientes.
4. Tener conexión a internet.

### Instalación
Ahora bien, para obtener el proyecto y ejecutarlo debe ser descargado en formato zip o puede ser clonado desde el repositorio de GitHub. 
Con el proyecto en su máquina, en su IDE de preferencia, debe seleccionar el directorio que contiene el proyecto y abrirlo. 
Luego, desde la terminal, debe descargar las dependencias del proyecto, para esto ejecute el comando `mvn install`. 
Después, para compilar ejecute el comando `mvn package` y por último ejecute el comando `java -cp .\target\classes\ edu.escuelaing.arem.ASE.app.HttpServer`.

## Despliegue
Con el proyecto corriendo debe abrir en un navegador la siguiente dirección: http://localhost:35000/movies.html allí podrá observar el *html* completo, que fue traido desde el disco local.

## Diseño
Se tiene un servidor HTTP que escucha por el puerto 35000, el cual obtiene la URI de la solicitud, que sirve para determinar la ruta al recurso solicitado. Y por medio del método *httpClientHtml*
se genera la respuesta a la solicitud dependiendo de la ruta. De modo que, se identifica el tipo de recurso, entre *html*, *java script*, *css* e imagen *PNG* y se 
retorna la respuesta a la solicitud.

En cuanto a la distribución, se tienen dos carpetas, una con el código del servidor y otra que contiene los recursos *html*, *java script*, *css* e imagen *PNG* del disco local.

## Evaluación
Al ingresar la dirección http://localhost:35000/movies.html se muestra la página html que tiene css, script e imagen.

![image](https://github.com/JessicaDMunozO/Taller2-AREP/assets/123814482/1a42866c-f0d8-4241-b793-5fb057f66c3f)

Para solicitar el script se debe ingresar la dirección http://localhost:35000/moviesScript.js

![image](https://github.com/JessicaDMunozO/Taller2-AREP/assets/123814482/6c996c1b-b8b7-495f-8b17-c2d2d7f21097)

Para solicitar el css se debe ingresar la dirección http://localhost:35000/styles.css

![image](https://github.com/JessicaDMunozO/Taller2-AREP/assets/123814482/b76e4a34-7099-4eb8-8dba-608672afe839)

Y para solicitar la imagen PNG se debe ingresar la dirección http://localhost:35000/movie.png

![image](https://github.com/JessicaDMunozO/Taller2-AREP/assets/123814482/1f387d87-c3b9-4bd7-98a9-02143e1c4eea)

Por último, si ingresa un path erroneo se muestra

![image](https://github.com/JessicaDMunozO/Taller2-AREP/assets/123814482/c89ccb3c-0e45-4940-b03d-47c18e0f1617)

## Construido con
Maven - Gestión de dependencias

## Versiones
Git - Control de versiones

## Autor
Jessica Daniela Muñoz Ossa


