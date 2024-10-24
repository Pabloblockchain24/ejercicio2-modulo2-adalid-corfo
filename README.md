# Ejercicio 2 - Módulo 2 Adalid Corfo

## Descripción del Proyecto

Este proyecto es una práctica para el Módulo 2 del curso Adalid Corfo. Se trata de un sitio web simple que presenta un hospital médico con tres secciones principales: Home, Equipo Médico y Contacto. El objetivo es implementar un sitio web modular utilizando HTML, SCSS, y CSS, se han aplicado media queries y modularización de estilos mediante el uso de SASS para una estructura más clara y mantenible.

## Instrucciones para Visualizar el Proyecto

1. Clona el repositorio en tu máquina local:

    ```bash
    git clone https://github.com/Pabloblockchain24/ejercicio2-modulo2-adalid-corfo.git
    ```

2. Navega a la carpeta del proyecto:

    ```bash
    cd ejercicio2-modulo2-adalid-corfo
    ```

3. Instala las dependencias de SASS si aún no lo has hecho:

    ```bash
    npm install -g sass
    ```

4. Compila los archivos SASS:

    ```bash
    sass assets/styles/main.scss assets/styles/main.css
    ```

5. Abre el archivo `index.html` en tu navegador favorito para visualizar el proyecto.

## Estructura de carpetas y archivos

```
ejercicio1-modulo2-adalid-corfo/
│
├── index.html              # Página principal (Home)
├── pages/
│   └── equipoMedico.html   # Página del equipo médico
│   └── contacto.html       # Página de contacto              
├── assets/img/
│   └── [imágenes utilizadas en el proyecto]
├── assets/styles/
│   └── abstracts
│        └── _abstracts.scss  # Estilos parciales de breakpoints y variables
│   └── base
│        └── _fonts.scss      # Estilos parciales de fuentes y tamaños de letra
│   └── components
│        └── _buttons.scss    # Estilos parciales de botones
│   └── layout
│        └── _footer.scss    # Estilos parciales de footer
│        └── _header.scss    # Estilos parciales de header
│   └── pages
│        └── contacto.scss          # Estilos parciales para page contacto
│        └── _equipo-medico.scss    # Estilos parciales para page equipo-medico
│        └── _main.scss             # Estilos parciales para page main
│   └── themes
│        └── _theme-adalid.scss     # Estilos parciales para colores y tema de la web 
│   └── vendors
│        └── _reset.scss            # Estilos basicos e iniciales de la web
│   └── main.scss            # Archivo que une los scss parciales
└── estilos.css              # Archivo resultante del preprocesador sass
└── estilos.css.map          # Archivo resultante del preprocesador sass
└── README.md                # Instrucciones y descripción del proyecto
```

## Modularización de Estilos

La estructura de los estilos está organizada utilizando SASS, dividiendo los estilos en archivos parciales para mejorar la organización y modularidad del código. Los archivos parciales están agrupados por funcionalidades, como layout, componentes, páginas, temas, entre otros. 

- `abstracts/_variables.scss`: Define los breakpoint a utilizar.
- `base/_fonts.scss`: Contiene las definiciones de fuentes utilizadas en el proyecto.
- `components/_buttons.scss`: Define los estilos para los botones.
- `layout/_header.scss`: Estilos específicos para la cabecera.
- `layout/_footer.scss`: Estilos del pie de página.
- `pages/_contacto.scss`: Estilos específicos de la página de contacto.
- `pages/_equipo-medico.scss`: Estilos específicos de la página del equipo médico.
- `pages/_main.scss`: Estilos específicos de la página principal de la web
- `themes/_theme-adalid.scss`: Estilos para el colores y tema personalizado del sitio.
- `vendors/_reset.scss`: Contiene un reset CSS básico para normalizar estilos entre navegadores.

Todos estos archivos se importan en el archivo principal `main.scss`, que se compila en el archivo CSS final.

## Media Queries

Se han implementado media queries en varios de los archivos parciales para asegurar que el diseño sea completamente responsivo. Los principales puntos de ruptura (`breakpoints`) son:

- 1200px: Para pantallas grandes.
- 1024px: Para pantallas medianas.
- 768px: Para tabletas.
- 576px: Para tabletas pequeñas y moviles grandes
- 420px: Para moviles pequeños

Estos breakpoints se aplican en las secciones necesarias, como el layout y los componentes, para que el sitio funcione correctamente en diferentes tamaños de pantalla.

## Explicación de las vistas

- **Home (index.html):** Esta es la página principal del sitio. Contiene una bienvenida a los usuarios y una breve descripción del Hospital. Se incluyen enlaces de navegación a las otras secciones del sitio.
  
- **Equipo Médico (equipo-medico.html):** En esta sección se presenta al equipo de médicos del hospital. Cada miembro tiene su propia descripción, destacando su especialidad y experiencia.

- **Contacto (contacto.html):** Aquí se ofrece un formulario de contacto para que los usuarios puedan enviar mensajes o consultas al hospital. Se incluyen campos como nombre, correo electrónico y mensaje.

## Créditos

- Las imágenes utilizadas en este proyecto fueron obtenidas desde https://www.chatgpt.com



