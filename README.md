# Clasificación de imágenes (perros y gatos)

Este código fuente sirve como apoyo para el video de creación de un clasificador de perros y gatos usando Python y Tensorflow, del canal de YouTube [Ringa Tech](https://youtube.com/RingaTech)

Este código representa el sitio web, una vez que se crea y entrena el modelo de inteligencia artificial con Python y Tensorflow, el cual es exportado a los archivos "json" y "bin".
Puede utilizarse en el celular, solo apunta la cámara al perro o gato que quieres clasificar (puede ser una imagen de la computadora, una foto, o uno de verdad), lo hace todo en el explorador utilizando Tensorflow.js.

## Cómo utilizarlo

### Descargar el repositorio
Descarga el repositorio donde gustes en tu computadora

### Inicia un servidor en la carpeta
Este proyecto utiliza un modelo de Tensorflow.js, el cual para cargarse requiere que el acceso sea por medio de http/https.
Para eso puedes usar cualquier servidor, pero aquí hay una forma de hacerlo:
- Descarga Python en tu computadora
- Abre una línea de comandos o terminal
- Navega hasta la carpeta donde descargaste el repositorio
- Ejecuta el comando `python -m http.server 8000`
- Abre un explorador y ve a http://localhost:8000

### Utilizarlo en un celular
Si quieres abrirlo en tu celular, no se puede solo poner la IP local de tu computadora y el puerto, ya que para usar la cámara se requiere HTTPS. Puedes hacer un túnel de HTTPS siguiendo los siguientes pasos
- Descarga ngrok en tu computadora, y descomprímelo
- Abre una línea de comandos o terminal
- Navega hasta la carpeta donde descargaste ngrok
- Ejecuta el comando `ngrok http 8000`
- Es importante tener ambos activos: El servidor de python, y el túnel de ngrok
- En la línea de comandos aparecerá un enlace HTTPS. Puedes entrar ahí con tu celular, no importa si no estás en la red local.
- El túnel expira después de 2 horas creo, en dado caso solo reinicias ngrok
- Abre un explorador en tu celular y ve al enlace HTTPS indicado

### Uso
Puedes dar clic en el botón de "Cambiar camara" para utilizar la cámara delantera o trasera del celular. Solo apunta la cámara a un perro o gato, y abajo te aparecerá la predicción. Tampoco es el clasificador del futuro entonces si no clasifica perfecto, oops.

## Problemas
Si tienes un problema, regístralo aquí o déjame un comentario en el video de Youtube. Asegúrate de primero revisar la consola de desarrollador de tu explorador para ver si puedes identificar el problema.