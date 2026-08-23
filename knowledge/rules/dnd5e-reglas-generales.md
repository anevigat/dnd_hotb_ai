# Reglas generales de D&D (5ª edición) — conocimiento de referencia

> **Alcance**: esto NO es específico de Heroes of the Borderlands. Es una síntesis de las reglas generales de D&D 5ª edición, para usar como **base de conocimiento de respaldo** cuando el material de HotB no cubra una duda concreta (HotB es un starter set y no incluye todas las reglas). Ante cualquier conflicto, las reglas/cartas propias de HotB (`knowledge/rules/`, `knowledge/monsters/`, etc.) tienen prioridad; esto es solo el fallback general.
>
> **Fuente**: vídeo de YouTube "Aprende D&D en menos de 20 minutos | dRol 39" (canal dRol). Contenido sintetizado/reescrito a partir de la transcripción, no es una copia literal.

## El ciclo básico de juego

Todo D&D funciona con el mismo ciclo: el **Director de Juego (DJ/Master)** describe una escena → los jugadores dicen qué intentan hacer sus personajes → si hace falta, se tiran dados para resolver la incertidumbre → el DJ describe el resultado y la escena avanza. Se repite constantemente.

## La mecánica central: d20 + Clase de Dificultad (DC)

- Casi toda acción incierta se resuelve tirando un **dado de 20 caras (d20)**.
- El DJ fija una **Clase de Dificultad (DC)** para la acción (ej. DC 11 para esconderse en unas condiciones normales).
- Al resultado del dado se le suman **modificadores** (según la habilidad/atributo relevante del personaje).
- Si el total iguala o supera la DC, la acción tiene éxito.
- Cuanto más difícil sea la tarea, más alta la DC (ej. esconderse a plena luz del día podría requerir DC 16 en vez de 11).

## Ventaja y desventaja

Es la mecánica distintiva de la 5ª edición para modelar circunstancias favorables o desfavorables:
- **Ventaja**: se tiran dos d20 y se queda el resultado más alto.
- **Desventaja**: se tiran dos d20 y se queda el resultado más bajo.
- Si una misma tirada tiene ventaja y desventaja a la vez (de cualquier fuente, una o varias), se cancelan entre sí y se tira un solo d20 normal.

Además del d20, existen otros dados (d4, d6, d8, d10, d12) usados según arma, hechizo o efecto concreto.

## Combate

- Fuera de combate el tiempo es flexible (el DJ puede narrar que pasan horas, días, etc. libremente).
- En combate el tiempo se divide en **rondas de 6 segundos**, y cada participante (jugadores, aliados, enemigos) tiene un turno por ronda.
- **Iniciativa**: al empezar el combate, cada participante tira 1d20 + modificador de Destreza (u otro, según el caso); de mayor a menor resultado se define el orden de turnos.
- En su turno, un personaje normalmente puede:
  - **Moverse** (por defecto ~9 metros/30 pies) — puede repartir el movimiento antes/después de la acción.
  - **Tomar una acción**: atacar, correr, esconderse, ponerse a la defensiva, preparar una acción condicional ("si entra alguien, ataco"), lanzar un hechizo, etc. Algunas clases obtienen ataques múltiples con su acción.
  - **Acción extra / bonus action**: solo si una habilidad/hechizo específico dice explícitamente que funciona como tal; se hace además de la acción normal.
  - **Reacción**: se ejecuta fuera de tu turno, cuando se cumple un disparador. El ejemplo más común es el **ataque de oportunidad**: si un enemigo con el que estás en combate cuerpo a cuerpo se aleja sin cuidado, puedes reaccionar atacándolo. Sin una habilidad que otorgue reacciones, un personaje no tiene ninguna disponible por defecto.

### Resolver un ataque

- Funciona igual que cualquier tirada: d20 + modificadores de ataque, comparado contra la **Clase de Armadura (AC/CA)** del objetivo (el equivalente a la DC pero para golpear a alguien).
- Si el total iguala o supera la AC, el golpe conecta y aplica su efecto (normalmente daño).
- **20 natural** en el dado de ataque = **golpe crítico**: conecta automáticamente (ignora modificadores) y se duplican los dados de daño.
- **1 natural** en un ataque = **fallo automático**, sin importar los modificadores.

### Puntos de golpe (HP) y muerte

- Todo personaje tiene una reserva de **puntos de golpe (HP)**: una abstracción de cuánto daño/cansancio puede aguantar.
- Al llegar a 0 HP, el personaje cae inconsciente y entra en **riesgo de morir**.
- Si nadie lo atiende/estabiliza, cada ronda debe hacer una **tirada de salvación de muerte** (1d20, sin modificadores):
  - 10 o más: un éxito.
  - 9 o menos: un fallo.
  - 3 éxitos acumulados: se estabiliza automáticamente.
  - 3 fallos acumulados: el personaje muere.
  - **20 natural** en esta tirada: se levanta de inmediato con 1 HP.
  - **1 natural**: cuenta como dos fallos.
- Existen además **condiciones** (agarrado, derribado, aturdido, etc.) que añaden reglas específicas a la situación de combate; el DJ es quien las administra.

## La hoja de personaje

### Atributos (habilidades)

Seis atributos base, cada uno con un valor numérico (normalmente entre 3 y 18, con 10-11 como "promedio"):
- **Fuerza**: poder físico.
- **Destreza**: agilidad y precisión.
- **Constitución**: salud y resistencia física.
- **Inteligencia**: conocimientos y razonamiento.
- **Sabiduría**: percepción y sentido común.
- **Carisma**: fuerza de voluntad y proyección de personalidad ante otros.

Cada atributo genera un **modificador** que se aplica a las tiradas relacionadas. Se pueden generar tirando dados o repartiendo un set de valores predefinidos (para equilibrar entre personajes).

### Raza

Define la especie del personaje (humano, elfo, enano, halfling, dracónido, semiorco, etc.). Cada raza aporta tendencias de atributos, rasgos y ventajas propias.

### Clase y nivel

La clase define qué puede hacer el personaje (guerrero, mago, pícaro/ladrón, clérigo, paladín, druida, hechicero, monje, brujo/warlock, bardo, etc.). El nivel (de 1 a 20) mide experiencia y poder; un personaje puede subir de nivel en una sola clase o combinar niveles de varias clases ("multiclase"). Cada nivel otorga nuevas capacidades — el manual de reglas detalla qué se gana en cada nivel de cada clase.

### Trasfondo (background)

Historia previa del personaje (huérfano, noble, marino, etc.) que otorga conocimientos, competencias y una pequeña ventaja narrativa dentro del mundo de juego (acceso a bibliotecas, refugio, comida, etc.).

### Habilidades (skills)

18 habilidades predefinidas, cada una ligada a un atributo (ej. Sigilo → Destreza, Persuasión → Carisma, Religión → Inteligencia, Supervivencia → Sabiduría). Clase, trasfondo y otras opciones pueden dar entrenamiento/competencia extra en habilidades específicas, sumando otro modificador (ej. un ladrón experto en Sigilo puede tirar con un bono mucho mayor que otro personaje).

### Tiradas de salvación

Tiros ligados a los atributos que el DJ pide cuando corresponde (de Fuerza, Destreza, Constitución, etc.) para resistir un efecto. Algunas clases tienen competencia extra en tiradas de salvación específicas.

### Equipo

Todo lo que el personaje lleva (armas, mochila, munición, etc.) debe estar anotado en la hoja — un personaje solo puede usar lo que tiene registrado, y hay que llevar cuenta de consumibles (flechas, componentes, etc.). El tipo de arma determina el dado de daño usado en combate.

### Dotes/feats (regla opcional)

Al subir de nivel, muchas mesas permiten elegir dotes (feats) que dan beneficios adicionales — por ejemplo, "ataque poderoso": restar puntos al ataque a cambio de más daño si conecta.

### Personalidad y roleo

- **Alineamiento**: dos ejes — legal/neutral/caótico y bueno/neutral/malvado — que dan una idea general de cómo se comporta el personaje frente a las leyes y la moral, sin determinar su personalidad por completo.
- **Rasgos de personalidad, ideales, vínculos y defectos**: frases cortas (a menudo sugeridas por el trasfondo) que ayudan a interpretar al personaje de forma consistente.

## Hechizos (para clases con magia)

- Cada clase de lanzador de hechizos tiene acceso a una lista de hechizos propia, y según nivel puede lanzar cierta cantidad por día.
- **Componentes**: verbal (hay que poder hablar), somático (hay que tener las manos libres) y material (requiere un objeto/componente, algunos se consumen al usarse).
- **Tiempo de lanzamiento**: puede ser una acción completa, una acción extra (bonus action), o incluso minutos, según el hechizo.
- **Cantrips/trucos**: hechizos de nivel muy bajo que se pueden lanzar libremente, sin gastar usos diarios.
- **Concentración**: algunos hechizos duran varias rondas mientras el personaje se mantiene concentrado. Solo se puede mantener un hechizo de concentración a la vez, y recibir daño puede hacer que se pierda la concentración (y el efecto termine).

## Nota sobre alcance de esta síntesis

El propio vídeo aclara que esto es una introducción muy resumida (~20 minutos) y remite a las reglas básicas oficiales y a los manuales completos para profundizar. Úsalo como referencia rápida de mecánicas generales — no sustituye al material oficial ni a las reglas específicas de Heroes of the Borderlands cuando estas existan.
