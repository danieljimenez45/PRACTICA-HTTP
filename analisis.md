### Petición HTTP – URL A (https://librebits.info)

- **Método HTTP (GET):** Solicita un recurso al servidor sin enviar datos en el cuerpo.
- **Ruta (/):** Indica que se solicita el recurso principal del sitio web.
- **HTTP/2:** Versión del protocolo que mejora el rendimiento respecto a HTTP/1.1.
- **Host:** Dominio al que se dirige la petición.
- **User-Agent:** Identifica el navegador y sistema operativo del cliente.
- **Accept:** Especifica los tipos de contenido que el navegador puede procesar.

### Respuesta HTTP – URL A

- **200 OK:** El servidor ha procesado correctamente la petición.
- **Date:** Fecha y hora en la que el servidor generó la respuesta.
- **Server:** Indica el software del servidor web (nginx).
- **Content-Type:** El recurso devuelto es HTML.
- **Content-Encoding:** El contenido se envía comprimido con gzip.
- **ETag / Last-Modified:** Permiten al navegador gestionar la caché del recurso.


### Petición HTTP – URL B (https://librebits.info/404)

- **Método HTTP (GET):** Solicita un recurso inexistente en el servidor.
- **Ruta (/404):** Indica el recurso específico que no se encuentra disponible.
- **HTTP/2:** El navegador utiliza HTTP/2 para la comunicación.
- **Host:** Dominio al que se envía la petición.
- **User-Agent:** Identifica el cliente que realiza la solicitud.
- **Accept:** Define los tipos de contenido que el navegador acepta.

### Respuesta HTTP – URL B

- **404 Not Found:** El recurso solicitado no existe en el servidor.
- **Server:** Sigue siendo el mismo servidor, aunque el recurso no esté disponible.
- **Content-Type:** Normalmente HTML con una página de error.


### Petición HTTP – URL C (https://librebits.info/social.org)

- **Método HTTP (GET):** Solicita un recurso adicional del sitio web.
- **Ruta (/social.org):** Recurso concreto solicitado al servidor.
- **HTTP/2:** Protocolo utilizado para mejorar el rendimiento.
- **Host:** Dominio del servidor destino.
- **User-Agent:** Información del navegador y sistema operativo.
- **Accept:** Tipos de contenido que el cliente puede procesar.

### Respuesta HTTP – URL C

- **404 Not Found:** El recurso solicitado no existe en el servidor.
- **Server:** Servidor que procesa la petición (nginx).
- **Date:** Fecha y hora de generación de la respuesta.
- **Content-Type:** HTML con una página de error.


### Comparación de respuestas HTTP (A, B y C)

- **URL A (200 OK):** El recurso principal existe y se entrega correctamente.
- **URL B (404 Not Found):** El recurso no existe, pero el servidor responde correctamente.
- **URL C:** Muestra un comportamiento similar a A o B según la disponibilidad del recurso.
- En todos los casos se utiliza el mismo servidor web (nginx) y HTTP/2.


### Análisis DNS de librebits.info

- **Registro A:** Asocia el dominio con una dirección IPv4.
- **Nameservers:** Servidores responsables de resolver el dominio.
- **TTL:** Tiempo que los resultados se mantienen en caché.
- **DNS:** Permite traducir nombres de dominio a direcciones IP.
- **DNS es un sistema jerárquico y distribuido**, fundamental para el funcionamiento de Internet.


### Recurso Imagen (icon-192x192.png)

- **GET:** Solicita un recurso gráfico al servidor.
- **Content-Type: image/png:** Indica que el recurso es una imagen PNG.
- **Content-Length:** Tamaño del archivo en bytes.
- **Server:** Servidor web que entrega el recurso.
- **Accept-Ranges:** Permite la descarga parcial del recurso.
- **ETag / Last-Modified:** Facilitan la caché en el navegador.

### Recurso CSS (style.css)

- **GET:** Solicita una hoja de estilos al servidor.
- **Content-Type: text/css:** Indica que el recurso es una hoja de estilos.
- **Server:** Servidor web que entrega el archivo CSS.
- **Date:** Fecha y hora en la que se envía el recurso.
- **El CSS define la presentación visual del sitio web**, no su contenido.

### Comparación de Content-Type

- **text/html:** Documento principal que define la estructura del sitio web.
- **image/png:** Recurso gráfico utilizado por la página.
- **text/css:** Hoja de estilos que define el diseño y la apariencia visual.
este seria todo el analisis