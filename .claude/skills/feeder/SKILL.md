---
name: feeder
description: Ingiere material oficial de D&D Heroes of the Borderlands (PDFs, capturas/imágenes, vídeos de YouTube) y lo clasifica/archiva en la base de conocimiento del repo. Usar cuando el usuario pase un PDF, una imagen, o un link/transcripción de YouTube para añadir como contexto.
---

# Feeder — ingesta de conocimiento

Alimenta `knowledge/` y `dm-only/` a partir de material que el usuario proporciona. Sigue estos pasos:

## 1. Identifica el tipo de entrada

- **PDF**: ruta a un archivo `.pdf`.
- **Imagen(es)/capturas**: ruta(s) a `.png`/`.jpg`/etc.
- **Vídeo de YouTube**: un link, o el usuario pega directamente una transcripción/resumen.

## 2. Extrae el contenido

- PDF e imágenes: léelos directamente con la herramienta de lectura de archivos.
- Vídeo con link: intenta obtener la transcripción/subtítulos con una herramienta de fetch sobre la URL. Si no es posible obtener texto útil, dile al usuario que no se pudo extraer automáticamente y pídele que pegue la transcripción o un resumen manual — no sigas sin contenido real.
- Vídeo con transcripción ya pegada: úsala directamente.

## 3. Clasifica el contenido

Decide categoría: `rules`, `maps`, `characters`, `monsters`, o `video-notes` (para dinámica de vídeos).

Para vídeos, extrae específicamente **dinámica de juego** (ritmo de sesión, cómo se manejan combates, técnicas de narración/DM, errores a evitar) — no un resumen de la trama del vídeo salvo que sea relevante para jugar.

Decide también si el contenido **revela spoilers** (trama, secretos, soluciones, giros): si es así, va en `dm-only/` (en `plot-outline.md`, `secrets.md`, o un archivo nuevo si el volumen lo justifica) en vez de en `knowledge/`.

## 4. Escribe el archivo

Crea un `.md` limpio con el contenido extraído/resumido (no copies el PDF/imagen en crudo, sintetiza lo relevante para jugar), con un nombre descriptivo en kebab-case, dentro de la subcarpeta correspondiente.

## 5. Actualiza el índice

- Si fue a `knowledge/`: añade una fila a `knowledge/INDEX.md` (archivo, categoría, fuente, fecha, spoiler=no).
- Si fue a `dm-only/`: añade una fila a la tabla de `dm-only/README.md`.

## 6. Confirma al usuario

Resume en 1-2 frases qué se añadió y dónde, y si algo quedó pendiente (p. ej. no se pudo extraer la transcripción del vídeo).
