# Pocket — Plum-style Mobile UI

Réplica **pixel a pixel** de una pantalla de app fintech (estilo Plum): degradado púrpura que se
funde a blanco, tarjeta de balance, acciones rápidas, tarjetas de ahorro y bottom nav.
Solo la **UI interior** de la pantalla (sin bisel del teléfono), HTML + CSS puro, sin dependencias
ni build.

## Vista previa

Abre `index.html` en el navegador. En móvil ocupa toda la pantalla; en escritorio se muestra
centrada al ancho de un teléfono (420 px) sobre un lienzo lila.

## Estructura

```
plum-ui-clone/
├── index.html   # markup de la pantalla (status bar, header, balance, tarjetas, nav)
├── styles.css   # degradado, tipografía Poppins, tarjetas, iconos y bottom nav
└── README.md
```

## Detalles de diseño

- **Tipografía:** Poppins (Google Fonts), la sans geométrica redondeada que más se acerca a la de Plum.
- **Color:** degradado vertical `#45189e → #6321cf → #8b57e8 → #ffffff` que blanquea justo antes de "Pockets".
- **Iconos:** SVG en línea (stroke), sin librerías externas.
- **Componentes:** status bar con dynamic island, tarjeta *Pocket* tipo glass, 4 acciones
  (Deposit / Withdraw / Brain / Splitter), tarjetas *Cash ISA* y *Plum Interest*, sección *Pockets*
  y bottom nav con el botón de ahorros activo (negro).
- **Accesibilidad:** contraste alto, `aria-label` en botones de icono y `prefers-reduced-motion`.

## Uso

```bash
open index.html      # macOS
xdg-open index.html  # Linux
```

> UI de demostración con fines de práctica de diseño. "Plum" es marca de sus respectivos dueños.
