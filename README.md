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

Repositorio, después de cambiar el nombre: https://github.com/AnderssonEspinoza/AnderssonEspinoza.github.io

Sitio gratuito, después de configurar GitHub Pages: https://anderssonespinoza.github.io/

## Migración desde el dominio vencido

El dominio de Namecheap `anderssonespinoza.me` dejó de ser necesario para publicar el portafolio. Se eliminó el archivo `CNAME` y las URL canónicas y sociales ahora apuntan a `https://anderssonespinoza.github.io/`.

Pasos pendientes de administración (se realizan en la interfaz de GitHub):

1. En Settings > Pages, eliminar `anderssonespinoza.me` en **Custom domain**, si sigue configurado.
2. En Settings > General, cambiar el nombre de este repositorio a `AnderssonEspinoza.github.io` (respetando el usuario real de GitHub).
3. En Settings > Pages, verificar que publique desde `main` / `(root)` y que la dirección final sea `https://anderssonespinoza.github.io/`.
4. Probar idiomas, enlaces, imágenes, CV y formulario tras la publicación.

No es necesario contratar otro alojamiento ni pagar por un dominio propio.
