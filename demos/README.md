# Demos públicas para el portafolio

Versiones de demostración independientes de los sistemas de producción. Las pruebas no requieren registro.

## Proyectos y accesos

| Proyecto | Acceso desde el portafolio | Comportamiento |
| --- | --- | --- |
| ZeroDay | Enlace a la app pública | App real, sin cuenta obligatoria |
| ClientManager | `demos/clientmanager.html` | Crear lead ficticio, tomar lead, avanzar estado, ver indicadores, exportar CSV |
| ClientManager, vista original | Enlace a `/demo-publica/index.html` en su dominio | Páginas estáticas de solo lectura incluidas en el repositorio Laravel |
| UniHelp / Sherly | `demos/unihelp.html` | Crear pregunta, filtrar, responder, valorar y ganar puntos ficticios |
| SmartPOS | `demos/smartpos.html` | Ventas, baja de inventario, fiados, abonos, reposiciones y reportes |
| CodeWard AI | Enlace a app real | Modo invitado y ejemplo con datos simulados; las auditorías reales requieren backend disponible |

## Seguridad y límites

- Las tres demos propias del portafolio se ejecutan **100% en el navegador**, sin peticiones a servicios de los proyectos originales.
- Los datos iniciales son completamente ficticios y se guardan por separado mediante `localStorage` del origen de este portafolio. Usa «Reiniciar demo» para restaurarlos.
- No se reutilizan contraseñas, claves, tokens, base de datos, código fuente ni lógica de autorización de los proyectos privados.
- No son equivalentes completos a los productos. Solo reproducen **flujos representativos** para enseñar su utilidad.
- Los enlaces a los sistemas reales **no** omiten el login; mantienen su autenticación y sus permisos.
- La exportación CSV de ClientManager es una exportación local de datos ficticios. No corresponde a un reporte de un cliente real.
- El ejemplo de CodeWard es explícitamente **simulado**; no debe presentarse como una auditoría OSS real.

## Desarrollo y prueba manual

Desde la raíz del repositorio:

```bash
python3 -m http.server 8765
```

Prueba `http://localhost:8765/demos/clientmanager.html`, `/demos/unihelp.html` y `/demos/smartpos.html`:

1. Abre cada demo sin iniciar sesión.
2. Prueba una operación de escritura: crear lead, crear pregunta o registrar una venta.
3. Verifica que cambien los contadores, la tabla y las vistas relacionadas.
4. Recarga la página y confirma que la operación persiste solo en este navegador.
5. Usa «Reiniciar demo» y verifica la restauración de los datos iniciales.
6. Comprueba enlaces y navegación tanto en móvil como en escritorio.
7. Revisa la sección «Proyectos» en `index.html` y `en.html`.

## Publicación

Estos archivos se sirven directamente desde GitHub Pages, sin variables de entorno ni build. La integración del cambio en `main` publica las demos con los enlaces correspondientes.
