# Noche en el Cementerio · Halloween 2026

Invitación-juego para móvil. Web estática + Supabase.

- `index.html` — el juego. Cada invitado entra con su enlace personal: `/?i=CODIGO`.
- `panel.html` — panel de anfitriones: `/panel?i=CODIGO_ANFITRION`.
- `game.src.html` — fuente del juego (mismo archivo que el boceto en Claude). Tras editarlo: `./build.sh`.
- `config.js` — URL y clave publicable de Supabase (proyecto *aturi-stats*, esquema `halloween`).

Base de datos: tablas en el esquema `halloween` (no expuesto). La web solo llama a funciones `public.halloween_*`, que exigen el código del invitado.
