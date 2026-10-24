# Conecta TI 2026 · Kit de inicio U2S05

Sitio de un evento ficticio de tecnología. El HTML ya está completo y la hoja de estilos ya tiene colores, tipografía y bordes. **Lo que falta es la maquetación responsiva**, y eso es lo que vas a construir en esta sesión.

## Estructura

```
conecta-ti/
├── index.html          <- NO necesitas modificarlo (salvo el paso 1 del tutorial)
├── css/
│   └── estilos.css     <- aquí trabajas, en el bloque 6 al final del archivo
├── capturas/           <- aquí guardas tus 3 capturas de evidencia
└── README.md           <- aquí respondes la bitácora (al final de este archivo)
```

## Cómo abrirlo

- **En Codespaces:** sube la carpeta a un repositorio nuevo llamado `u2s05-conecta-ti`, abre el Codespace y ejecuta en la terminal `php -S localhost:8000`. Abre el puerto 8000 en el navegador.
- **Sin Codespaces:** abre `index.html` directamente en Chrome o Edge. Funciona igual porque es HTML y CSS puro.

## Anchos de prueba (DevTools, modo dispositivo)

| Vista | Ancho | Nombre de la captura |
|---|---|---|
| Celular | 375 px | `capturas/movil-375.png` |
| Tableta | 768 px | `capturas/tableta-768.png` |
| Escritorio | 1280 px | `capturas/escritorio-1280.png` |

Para tomar captura de página completa en DevTools: `Ctrl + Shift + P` (en Mac `Cmd + Shift + P`), escribe `screenshot` y elige **Capture full size screenshot**.

## Bitácora (responde aquí, 2 a 4 líneas por pregunta)

1. **¿Por qué el sitio original se veía diminuto o con barra horizontal en el celular? Menciona las dos causas que corregiste.**

   _Tu respuesta:_Falta de la etiqueta viewport: Sin ella, el celular intentaba mostrar una pantalla de escritorio completa, haciendo que todo se viera diminuto.

Falta de diseño Mobile First: Los elementos venían sin distribución responsiva (Flexbox o Grid), por lo que se desbordaban horizontalmente en pantallas pequeñas.

2. **¿En qué parte del sitio elegiste Flexbox y en cuál Grid? Explica el criterio que usaste (una dimensión vs. dos dimensiones).**

   _Tu respuesta:_Flexbox (1 dimensión): En elementos que se alinean en una sola dirección (como menús, la hora y el detalle de la agenda, o los patrocinadores).

Grid (2 dimensiones): En secciones que controlan filas y columnas al mismo tiempo (como la estructura de la agenda con áreas nombradas, los ponentes y el pie de página).

3. **¿Qué hace exactamente `repeat(auto-fit, minmax(240px, 1fr))`? Explícalo como si se lo contaras a un compañero que faltó.**

   _Tu respuesta:_minmax(240px, 1fr): Establece un ancho mínimo de 240px por tarjeta y hace que crezcan (1fr) si sobra espacio.

auto-fit: Ajusta automáticamente el número de columnas según la pantalla; si no caben, bajan de renglón solas sin usar media queries.

4. **¿Qué fue lo que más te costó y cómo lo resolviste? (qué recurso usaste: tutorial, hoja de referencia, checklist de errores, laboratorio, un compañero)**

   _Tu respuesta:_la ultima parte porque no me aceptaba los comandos en la parte de console y le tube que preguntar a la ia

---
*Conecta TI 2026 es un evento ficticio creado con fines didácticos. Prof. Alonso · Tecnologías de Información*
