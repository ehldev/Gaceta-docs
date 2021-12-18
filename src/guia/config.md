# Configuración principal

En la raíz del proyecto encontrará un archivo llamado env.js, el cual contiene
información importante y global del proyecto.

El archivo env tiene la siguiente estructura (Puede variar según la versión)

```js
export const appConfig = {
  graphUrl: "https://api.gacetajuridica.com.pe/graphql", // Endpoint Graphql
  cookieToken: "gctoken", // Nombre de cookie
  cookieDatosUsuario: "gj_user", // Nombre de cookie

  logoGacetaJuridica: "/imagenes/logo-gaceta-juridica.svg",

  openGraph: {
    urlOficial: "https://gaceta.josejollja.com",
    title: "Gaceta Jurídica",
    description: "Descripción de Gaceta Jurídica",
    image: "logo-gaceta",
    keywords: "Keywords Gaceta",
  },

  whatsapp: {
    numero: "+51997576053",
    mensaje: "",
  },

  publicaciones: {
    paginacion: 10,
  },
};
```

La mayoría de las propiedades son bastantes descriptivas en cuando a las otras, se detallan a continuación.

**logoGacetaJuridica:** Url relativa del logo principal que se mostrará en la app

**openGraph:** Muestra la configuración inicial o por default para todas las páginas dónde no se especifiquen.

Son datos importantes para el SEO de la web.

**whatsapp:** Número y mensaje que se mostrará en el botón flotante de whatsapp.

**publicaciones:** Contiene información general sobre como se mostrarán las publicaciones.

Por ejemplo el número de elementos que se obtendrán en la carga inicial y en cada paginación.
