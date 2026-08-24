---
name: session-prep
description: Prepara una misión/escenario concreto de D&D Heroes of the Borderlands antes de jugarlo. Recibe como argumento el nombre de la misión, región o encuentro (p. ej. "Cueva K" o "Duendes duelistas") y devuelve componentes necesarios, historia para narrar, tips de mesa, un paso a paso de cómo puede evolucionar la sesión, y una tabla de monstruos con iniciativa/CA/PG/daño. Usar cuando el usuario pida preparar, planificar o repasar antes de jugar un encuentro o región concreta.
---

# Session prep

Este skill es de uso exclusivo del DM (el usuario) — el resultado puede incluir spoilers de `dm-only/`, pero deja siempre marcada con claridad la parte "para leer en voz alta" (esa sí es apta para los jugadores) frente al resto (solo para el DM).

## 1. Localiza el escenario

Con el argumento recibido (nombre de misión/región/encuentro):

- Busca primero en `dm-only/` (grep por el nombre en `la-espesura/`, `cuevas-del-caos/`, `plot-outline.md`, `rumores-pnj.md`, etc.) — ahí está la trama, los componentes y las soluciones.
- Si el argumento es ambiguo o no aparece en ningún archivo, pídele al usuario que aclare o que confirme el nombre exacto antes de seguir — no inventes un encuentro que no esté en la base de conocimiento.
- Si el encuentro incluye monstruos/PNJs con carta propia, localiza sus stats en `knowledge/monsters/bestiario-monstruos.md` y las armas relevantes en `knowledge/items/equipo.md` (para el dado de daño + modificador de característica).
- Ten en cuenta el estado actual de la campaña (`campaign/state/world-state.md`, fichas en `campaign/party/`) para adaptar el output al grupo real (nivel, PG máximos, objetos que ya tienen, decisiones previas relevantes).

## 2. Genera el output con estas secciones, en este orden

### Componentes necesarios
Lista de todo lo físico/de referencia que hace falta tener a mano: póster de mapa, cartas de PJ/monstruo/objeto, mazos, fichas de poder, etc. (normalmente están indicados en la línea "Componentes" del encuentro en `dm-only/`; si no está indicada, infiere lo mínimo razonable a partir de lo que aparece en la escena).

### Historia para contar a los jugadores
Un texto breve, evocador, en 2do plural o al estilo "leer en alto" de las cartas de región — **sin ningún spoiler** (nada de soluciones, motivaciones secretas de PNJs, ni trampas ocultas). Es el texto que el DM puede leer o parafrasear directamente a la mesa para abrir la escena.

### Tips para que la sesión sea más divertida
3-5 consejos concretos y accionables (con el porqué breve si no es obvio): cómo repartir protagonismo, qué pistas dar si se atascan (siguiendo el protocolo de pistas graduales del proyecto), cómo ajustar la dificultad si el grupo va muy fuerte o muy flojo, momentos para pausas dramáticas, etc. Prioriza siempre que el encuentro sea desafiante pero no frustrante.

### Cómo puede evolucionar la sesión (paso a paso)
Un árbol breve de las ramas plausibles: qué pasa si negocian con éxito, si fallan, si van directo al combate, si el grupo pierde el combate, qué triggers de trama se activan (referenciando `dm-only/plot-outline.md` si aplica), y cualquier gancho que quede abierto según el resultado. Esta sección es solo para el DM (puede contener spoilers).

### Tabla de monstruos (si aplica)
Si el encuentro tiene monstruos o PNJs hostiles con carta de combate, una tabla:

| Nombre | Iniciativa | CA | PG | Ataques (daño) |
|---|---|---|---|---|
| ... | ... | ... | ... | arma 1 (dado+mod), arma 2 (dado+mod), ... |

Saca los valores de `knowledge/monsters/bestiario-monstruos.md` (iniciativa/CA/PG/mods) y de `knowledge/items/equipo.md` (dado de daño + modificador de cada arma que porte). Si algún dato no está en la base de conocimiento, dilo explícitamente en vez de inventarlo, y sugiere añadirlo con `/feeder`.

## 3. Confirma al usuario

Al final, resume en una frase si algo quedó sin poder resolver (encuentro no encontrado, monstruo sin stats en la base de conocimiento, etc.) para que el usuario sepa qué falta antes de sentarse a jugar.
