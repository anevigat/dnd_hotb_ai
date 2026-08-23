---
name: session-end
description: Cierra la sesión de juego actual de D&D Heroes of the Borderlands. Escribe el resumen de sesión, actualiza el estado persistente del mundo y las fichas de personajes. Usar cuando el usuario diga que van a terminar de jugar por hoy.
---

# Session end

## 1. Repasa lo ocurrido

Usa `campaign/state/current-session.md` (notas rápidas, HP final, condiciones) y el contexto de la conversación de esta sesión.

## 2. Escribe el resumen de sesión

Crea `campaign/sessions/session-NN-summary.md` (siguiente número disponible) siguiendo el formato de `campaign/sessions/README.md`: resumen de 3-6 frases, eventos clave, estado al cierre, ganchos abiertos. **Sin spoilers de `dm-only/`** — este resumen es apto para que los jugadores lo relean.

## 3. Actualiza el estado persistente

En `campaign/state/world-state.md`: nuevas entradas o cambios en misiones, PNJs conocidos, lugares/elementos del mapa, decisiones clave del grupo.

## 4. Actualiza fichas de personajes

Si hubo cambios de nivel/capítulo, equipo nuevo, o rasgos desbloqueados, actualiza el archivo correspondiente en `campaign/party/`.

## 5. Reinicia el tracker en vivo

Deja `campaign/state/current-session.md` limpio (HP/inventario actual quedan reflejados como el "estado de partida" para que `/session-start` los recoja la próxima vez; las notas rápidas en bruto se vacían porque ya están destiladas en el resumen).

## 6. Confirma al usuario

Indica qué archivos se actualizaron y muestra brevemente el resumen de sesión generado.
