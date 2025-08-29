

### SEO - Search Engine Optimization
    - Un conjunto de estrategias y técnicas utilizadas para mejorar la visibilidad de un sitio web en los diferentes motores de busqueda (Google, Brave, Bing..)


### Objetivos:
    - Aumentar el tráfico orgánico.
    - Mejorar la experiencia del usuario (UX)
    - Incrementar la presencia de lsitio.
    - Generar conversiones de calidad.

### Tipos de SEO:
    - SEO on-page: optimizaciones dentro del sitio web.
    - SEO off-page: Se relaciona a factores externos (redes sociales)
    - SEO técnico: Aspecto más relacionado con herramientas y conceptos ténicos que exigen los diferentes buscadores.


### SEO on-page:

    Elementos claves:
        - Contenido de calidad: relevante, único, diferenciandonos de la 'competencia' y que le agrega valor a la temática tratada.
        - Palabras claves: Trabajo de investigación, y uso estratégico para resaltar los puntos más importantes.
        - Estructura del sitio: Organización del contenido de forma lógica, amigable y facilmente navegable.
        - Experiencia de usuario (UX): Usabilidad y el diseño intuitivo.

### Proceso de investigación sobre palabras claves:
1. Identificar los temas principales.
2. Utilizar herramientas como Google Keywork Planner.
3. Analizar la competencia.
4. Distribuir las palabras claves de forma estrategica dentro del contenido.


### HTML Semántico y SEO

    Es muy importante utilizar las diferentes etiquetas HTML para representar el contenido de forma coherente con ellas.
    Es importante tener en cuenta la jerarquía de los encabezados, <h1> sabes que es el encabezado más relevante y solo podemos utilizarlo una vez por página. <h2> subtitulo importane / titulo de sección, <h3> subcontenedores / subsecciones...

### Meta tags: 
    - Nos permite agregan información extra sobre el sitio en cuestion, principalmente se utilizan a través de los robot's de los motores de busqueda.

***title***: Define el título de la página
<meta name="title" content="Titulo atractivo. | nombre de la marca">

***description***: Define una breve descripción del contenido principal que se ofrece en el sitio.
    - Longitud: 50-60 carácteres.
    - Contiene palabras claves más importantes.
    - Unico: debe ser diferente para cada página.

***keywords***: Son palabras claves sueltas, actualmente no tiene mucha relevancia aunque es recomendable colocarlas.

***Open Graph***: Nos permiten establecer el contenido a mostrar por ej, a la hora de compartir un sitio web a través de diferentes redes sociales (whatsapp y facebook).

<meta property="og:title" content="Titulo a mostrar al compartir">
<meta property="og:description" content="Descripción a mostrar al compartir">
<meta property="og:image" content="url_imagen">
<meta property="og:url" content="URL_de_la_pagina">
<meta property="og:website" content="website">

***Twitter Cards***:

<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:title" content="Titulo a mostrar cuando se comparte el link en twitter.">
<meta name="twitter:description" content="Descripción a mostrar cuando se comparte el link en twitter.">
<meta name="twitter:image" content="URL_image">


### Optimización de CSS para SEO:

    Cómo impacta el CSS en el SEO?
    - Velocidad de carga: el CSS que está optimizado mejora el rendimiento de carga del sitio.
    - Experiencia de usuario: Diseño responsive y accesible.
    - Core Web Vitals: Métricas medidas por Google para la experiencia de usuario.

1. Minificación de archivos CSS:
````css
/* Antes */
body {
    margin:0;
    padding:0;
    box-sizing:border-box;
}
/* minificado */
body{margin:0;padding:0,box-sizing:border-box;}
````

2. CSS critico: Utilizar unicamente aquel css que se utiliza para la parte visible de una página sin hacer scroll (above the fold). Podemos implementarlo utilizando los estilos 'criticos' cargandolos dentro de la etiqueta <head> y la etiqueta correspondiente para aplicar estilos <style>.

3. Diseño responsive: el uso e implementación de media querys.



### Estructura de URLs y navegación.

Es muy importante utilizar lo que se llama URLs Friendly. Urls Amigables.
Las URLs deben ser:
- Descriptivas: debe reflejar el contenido de la página.
- Cortas: Faciles de recordar y compartir.
- Guiones para separar palabras. Guiones medio, no guion bajo.
- Minisculas.

Ejemplos:
Mal: https://miweb.com/page.html?id=5
Mejorada: https://miweb.com/curso-seo-web

Navegación:
```html
<nav aria-label:"Navegación principal">
    <ul>
        <li><a href="/" title="Inicio">Home</a></li>
        <li><a href="/" title="Nuestros productos">Productos</a></li>
        <li><a href="/" title="Blog de noticias">Blog</a></li>
        <li><a href="/" title="Form de contacto">Contacto</a></li>
    </ul>
</nav>
```

### Optimización de la imagenes

    Importancia:
    - Mejorar la velocidad de carga.
    - Aumenta la accesibilidad
    - Mejora la oportunidad de ranking en busquedas de imágenes.

    Técninas a implementar:
    - Definir atributos title y alt
        <img alt="descripción" title="el titulo de la imagen" loading="lazy">
    - Utilizar formatos modernos: en lugar de utilizar .jpg o .png, actualmente se recomienda utilizar Webp, o AVIF. Igualmente es recomendable mantener archivos en formato jpg como alternativa, porque hay ciertos navegadores que todavía no soportan dicho formato, cómo podría implementar esta forma?
    <picture>
        <source srcset="imagen.webp" type="image/webp">
        <source srcset="imagen.avif" type="image/avif">
        <img src="imagen.jpg" alt="Descripción">
    </picture>  
    
    - Lazy loading nativo: Nos permite cargar las imagenes de forma 'diferida' ya que se van a cargar a medida que la imagen ingresa al area de visión del usuario.
       <img alt="descripción" title="el titulo de la imagen" loading="lazy">
       