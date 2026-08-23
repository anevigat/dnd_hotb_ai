# DM Copilot — D&D: Heroes of the Borderlands

Plantilla de repo para convertir a [Claude Code](https://claude.com/claude-code) en un asistente/co-DM para partidas de **D&D: Heroes of the Borderlands** (el starter set cooperativo de introducción a Dungeons & Dragons, basado en "Keep on the Borderlands").

Te ayuda a preparar sesiones, crear personajes, dirigir la partida turno a turno, describir escenas y PNJs, dar pistas a jugadores atascados sin espoilear la trama, y mantener el hilo de una campaña entre sesiones.

## Cómo funciona

- **[`CLAUDE.md`](./CLAUDE.md)** define el rol, el tono y los protocolos de trabajo (spoilers, pistas, estado en vivo).
- **`knowledge/`** es la base de conocimiento del juego: reglas, mapas, personajes pregenerados, monstruos y dinámica de mesa extraída de vídeos. Se alimenta con el skill `feeder`.
- **`dm-only/`** guarda trama y secretos — nunca se lee en voz alta a los jugadores.
- **`campaign/`** es el estado de tu partida en curso: fichas de personajes (`party/`), estado en vivo de HP/inventario/mapa (`state/`) y resúmenes de sesión (`sessions/`).
- **`.claude/skills/`** trae tres skills:
  - `feeder` — ingiere PDFs, capturas o vídeos de YouTube (vía `yt-dlp`) y los clasifica en `knowledge/` o `dm-only/`.
  - `session-start` — recap de la última sesión y carga del estado al empezar a jugar.
  - `session-end` — cierra la sesión: resumen, actualización del estado persistente y de las fichas.

## Para empezar

1. Clona este repo y ábrelo con Claude Code.
2. Usa `/feeder` para pasarle el material oficial del set (manual, mapas, cartas de personajes/monstruos) y así rellenar `knowledge/`.
3. Pide ayuda para crear los personajes del grupo — se guardan en `campaign/party/`.
4. Usa `/session-start` y `/session-end` en cada sesión de juego para no perder el hilo de la campaña.

## Aviso

- El material oficial de D&D: Heroes of the Borderlands (manuales, mapas, cartas) tiene derechos de autor de Wizards of the Coast. Este repo no incluye ese contenido; tú lo alimentas localmente con tu copia del juego, y lo que se guarda en `knowledge/` son síntesis/notas propias, no copias literales.
- `dm-only/` y `campaign/` contienen la trama y el estado de una partida concreta — si vas a compartir tu propia copia de este repo públicamente, revisa que no filtres spoilers de tu campaña ni datos personales de tu grupo de juego.
