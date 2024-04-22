# frame_js

- Marcos (iframes) en JavaScript

En JavaScript, el término "marcos" se refiere principalmente a la interacción con el elemento HTML <iframe>, que te permite incrustar contenido externo u otro documento HTML dentro de tu página web. Veamos a detalle qué son los marcos (iframes) y cómo interactúa JavaScript con ellos:

- Entendiendo los Marcos (iframes):

Los marcos (iframes) son elementos HTML que crean un contenedor dentro de tu página web para mostrar contenido de otra fuente, como un documento HTML separado, una imagen o un video.
Esto te permite exhibir contenido de fuentes externas sin problemas dentro de tu propia página.

- El Papel de JavaScript con los Marcos:

Si bien JavaScript no crea marcos directamente, proporciona funcionalidades potentes para interactuar con los iframes existentes incrustados en un documento HTML.

- JavaScript ofrece métodos y propiedades para:


- Acceder al Contenido del Marco:
Recuperar contenido de un marco usando su propiedad frameElement.contentDocument o el objeto frameElement.contentWindow.document.

- Modificar el Contenido del Marco:
Cambiar dinámicamente el contenido que se muestra dentro de un marco manipulando sus elementos DOM con técnicas JavaScript como querySelector(), textContent, etc.

- Comunicarse entre Marcos:

JavaScript permite la comunicación entre el documento principal (la página que contiene el iframe) y el contenido dentro del iframe (y viceversa) utilizando técnicas como:

    postMessage(): Enviar mensajes entre el documento principal y el iframe de forma asíncrona.

    Eventos de ventana: Responder a eventos activados dentro del contenido del iframe.

    Variables compartidas (usar con precaución debido a problemas de seguridad): Compartir variables accesibles tanto para el documento principal como para el iframe.

- ejemplo #1
(iframe)
    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
 <iframe src="https://es.wikipedia.org/wiki/Wikipedia:Portada" frameborder="10" width="400" height="400""></iframe>
 <iframe src="https://television.libre.futbol/tv2/" frameborder="10" width="400" height="400""></iframe>
 <iframe src="https://television.libre.futbol/tv2/" frameborder="10" width="400" height="300""></iframe>
 <iframe src="https://television.libre.futbol/tv2/" frameborder="10" width="400" height="200""></iframe>

</html>