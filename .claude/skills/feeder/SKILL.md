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
- **Vídeo con link de YouTube**: usa `yt-dlp` (herramienta instalada en el sistema) para extraer los subtítulos sin descargar el vídeo:

  ```bash
  # Subtítulos manuales en español (si el vídeo los tiene)
  yt-dlp --write-sub --skip-download --sub-lang es "URL"

  # Si no hay manuales, usar los autogenerados (caso más común)
  yt-dlp --write-auto-sub --skip-download --sub-lang es "URL"

  # Convertir a texto plano más fácil de leer
  yt-dlp --write-auto-sub --skip-download --sub-lang es --convert-subs srt "URL"
  ```

  Ejecuta esto en el directorio scratchpad de la sesión (no en el repo). El `.srt` resultante trae numeración y timestamps: límpialo antes de leerlo, por ejemplo:

  ```bash
  grep -vE '^[0-9]+$|-->|^$' archivo.srt | awk '!seen[$0]++' > archivo_plain.txt
  ```

  Si `yt-dlp` no está instalado o falla (vídeo privado, sin subtítulos en ningún idioma), dile al usuario y pídele que pegue la transcripción o un resumen manual — no sigas sin contenido real.
- Vídeo con transcripción ya pegada por el usuario: úsala directamente.

**Importante (derechos de autor)**: nunca copies la transcripción literal a los archivos del repo. Léela, y escribe una síntesis/resumen en tus propias palabras de lo relevante para jugar (reglas, dinámica, ideas) — igual que con PDFs e imágenes en el paso 4.

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
