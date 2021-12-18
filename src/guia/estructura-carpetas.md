# Estructura de carpetas

**/data** Contiene 3 archivos con información general de productos y módulos.

**/data/lista-productos.js** Contiene información general de los productos, algunas propiedades tienen comentarios descriptivos y otras se detallarán debajo de la imagen.

```js
{
    id: 1, // Id asignado, también reconocido por el backend
    idBackend: "GAC-CIVIL",
    idParaRedirigirASoftware: 'GacetaCivil',
    logo: "/imagenes/productos/civil/logo-civil.svg", // Logo principal del producto
    nombre: 'Gaceta Civil & Procesal Civil',
    text: "Gaceta Civil & Procesal Civil",
    descripcion: "Descripcion Gaceta civil",
    imagenPrincipal: "/imagenes/modulos/noticias/fondo-noticias.png",
    image: "/iconos-productos/gaceta-civil.svg",
    imageOpacity: "/iconos-productos/gaceta-civil-opacity.svg",
    tag: 'civil',
    nombreCarpetaEnPaginas: 'noticias-informes-opiniones', // Nombre de la carpeta en el directorio pages
    route: "/gaceta-civil-procesal-civil",
    logoZonaSuscriptores: '/productos/suscriptores/logo-civil.svg',
    rutaTrastienda: '/productos/trastienda/civil',
    modulos: [1, 2, 3, 4, 5, 6, 7, 8, 9, 15, 16], // Id de cada módulo a encontrar en modulos.js
    openGraph: {
        urlOficial: '',
        keywords: 'Keywords Gaceta civil',
        image: 'Image Gaceta civil',
        whatsappImage: 'Image whatsapp Gaceta civil'
    }
}
```

- _idBackend:_ El código que se usará comparar y permitir o no el ingreso a ciertas publicaciones según el producto.

- _tag:_ Identificador rápido principalmente para ser utilizado dinámicamente en clases css.

- _modulos:_ Lista de identificadores de los módulos que pertenecen al producto. Los módulos se encuentran en _./data/lista-modulos.js_ y se asignan al ingresar a la página _./pages/productos/\_slug_ la cual muestra la lista de módulos.

<img :src="$withBase('/images/estructura-carpetas/lista-modulos.png')" alt="foo">

<br />
<br />
<br />

**/data/lista-productos-menu.js** Contiene información general de los productos que se mostrarán en el menu.

**/data/lista-modulos.js** Contiene información general de los módulos.

**/static** Contiene archivos estáticos que usará la aplicación como el favicon.ico, logos o íconos.

...

**Los demás archivos son propios del Framework [Nuxt](https://nuxtjs.org/)**
