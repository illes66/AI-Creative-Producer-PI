# AI-Creative-Producer-PI
Easy playable in html5 for job candidacy

## Playable rápido (cozy, pocos segundos)
- Abre `index.html` en navegador.
- Controles: `← → ↑ ↓` o ratón/touch para mover el anzuelo.
- Objetivo corto: pescar 5 peces para ver el mensaje de clear.

## Dónde cambiar imágenes y animaciones
Todo está señalado dentro de `index.html`:
- `ASSET_PATHS`: rutas a PNG (`rod`, `hook`, `plants`, `fishes[]`).
- `GAME_CONFIG`: velocidad/cantidad de peces y duración de destellos.
- Giro de peces al dar la vuelta: en `drawFish()` con `ctx.scale(facingRight ? 1 : -1, 1)`.
- Destellos + popup de captura: en `spawnSparkles()`, `spawnCatchPopup()` y `state.popups`.

Si una imagen no existe aún, el juego usa dibujos fallback para que siga funcionando.
