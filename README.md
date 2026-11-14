# Portafolio de Andersson Espinoza

Portafolio estático en español (`index.html`) e inglés (`en.html`), basado en el diseño y los efectos de `portafolio-andersson-v6.html`.

HTML, CSS y JavaScript nativos, sin compilación ni dependencias de ejecución. Las fuentes se cargan desde Google Fonts.

## Desarrollo local

```sh
python3 -m http.server 8765
```

Abre http://localhost:8765. El estilo compartido está en `css/portfolio-v6.css`; los datos, animaciones e interacciones están en `js/portfolio-v6.js` y `js/portfolio-v6-en.js`.

## Comportamiento

- Navegación lateral en escritorio e inferior en celular y tablet.
- Arranque tipo terminal, credencial animada, ticker y eventos etiquetados como simulación.
- Servicios con interruptores y proyectos desplegables accesibles por teclado.
- Soporte para movimiento reducido y áreas seguras del dispositivo.
- Formulario conectado al endpoint Formspree existente, con validación y estados de envío, éxito y error. La entrega depende del servicio Formspree.

## Verificación

Revisado en navegador con anchos de 320, 390, 768, 1024 y 1440 píxeles. Se comprobaron desbordamiento horizontal, interruptores, acordeón, versión inglesa y movimiento reducido. Los estados del formulario se verificaron interceptando la solicitud con respuestas simuladas de éxito y error.

## Publicación

Repositorio: https://github.com/AnderssonEspinoza/anderssonespinoza.me

Dominio configurado en `CNAME`: https://anderssonespinoza.me
