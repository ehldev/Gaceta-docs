# Landings

Cada producto tiene asignado una Landing page.

Cada landing consta de un archivo de configuración y además una carpeta con las imágenes respectivas.

### Archivo de configuración

**Ruta:**
_/data/landings/Nombre de producto_

En cada archivo (según el producto) se encuentra información que podrá cambiar y ver reflejada en la vista de la Landing.

**_Por ejemplo:_**

> Si deseo cambiar algún texto del banner principal de Gaceta Civil & Procesal Civil:

<img :src="$withBase('/images/landings/banner-civil.png')" alt="Banner">

Tendré que situarme en la carpeta _/data/landings/civil_ y en ese archivo buscar la sección correspondiente, en este caso _"Banner"_ o _"carouselPrincipal"_

### Carpeta para imágenes

**Ruta:**
_/static/landing/Nombre de producto_

Dentro de la carpeta perteneciente al producto se encuentran distintas carpetas organizadas para cada sección relevante de cada landing.

**_Por ejemplo:_**

> Si deseo cambiar o añadir alguna imagen del banner principal de Gaceta Civil & Procesal Civil:

<img :src="$withBase('/images/landings/banner-civil.png')" alt="Banner">

Tendré que situarme en la carpeta _/static/landing/civil/banner_ y agregar o cambiar archivo.

El nombre del archivo a cambiar o agregar tiene que ser el mismo que el que se especificó en el archivo de configuración (Revisar ejemplo anterior)
