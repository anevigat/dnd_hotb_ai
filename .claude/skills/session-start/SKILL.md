---
name: session-start
description: Abre una nueva sesión de juego de D&D Heroes of the Borderlands. Carga el estado de la campaña, da un recap al DM y prepara el tracker en vivo. Usar cuando el usuario diga que va a empezar a jugar/dirigir una sesión.
---

# Session start

## 1. Lee el estado existente

- El último `campaign/sessions/session-NN-summary.md` (si existe alguno).
- `campaign/state/world-state.md`.
- `campaign/state/current-session.md` (por si quedó algo sin cerrar de una sesión anterior — avisa al usuario si es el caso).
- Las fichas en `campaign/party/`.

## 2. Da un recap breve al usuario (DM)

En pocas frases: dónde quedó la trama, estado del grupo (HP/recursos si son relevantes), ganchos abiertos, y cualquier misión o PNJ pendiente de `world-state.md`. Si el usuario lo pide, también puedes consultar `dm-only/` para recordarle secretos relevantes a esta sesión — solo a él, no en texto para leer a los jugadores.

## 3. Prepara el tracker en vivo

Reinicia/actualiza `campaign/state/current-session.md`:
- Número de sesión (incrementa desde la última) y fecha.
- Carga HP/condiciones/inventario de partida desde el cierre anterior (o desde las fichas de `campaign/party/` si es la primera sesión).
- Limpia la sección de "notas rápidas" para esta nueva sesión.

## 4. Confirma que estás listo

Dile al usuario que el estado está cargado y que puede empezar a narrar/jugar; recuérdale que irás actualizando `current-session.md` a medida que ocurran cosas.
