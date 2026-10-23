---
name: stop-slop-es
description: Elimina los patrones de escritura de IA en textos en español. Úsala al redactar, editar o revisar posts, correos, mensajes o cualquier texto para quitar las marcas predecibles de la IA.
metadata:
  trigger: Redactar prosa en español, editar borradores, revisar contenido en busca de patrones de IA
  author: Hardik Pandya (https://hvpandya.com)
  original: https://github.com/hardikpandya/stop-slop
  adapter: Wassim Aarab (https://github.com/WassimAarab08)
  language: es
---

# Stop Slop (español)

Elimina de la prosa los patrones predecibles de la escritura generada por IA.

## Reglas principales

1. **Quita el relleno.** Fuera las aperturas de calentamiento, las muletillas de énfasis, la jerga corporativa y los adverbios. Ver [references/phrases.md](references/phrases.md).

2. **Rompe las estructuras de fórmula.** Evita los contrastes binarios ("No es X, es Y"), las listas en negativo, la fragmentación dramática, las preguntas retóricas de arranque y la agencia falsa. Ver [references/structures.md](references/structures.md).

3. **Usa la voz activa.** Cada frase necesita un sujeto humano que haga algo. Nada de pasivas ("fue aprobado") ni de pasivas con "se" que esconden al responsable ("se tomó la decisión"). Nada de objetos que hacen cosas de personas ("la queja se convierte en mejora").

4. **Sé concreto.** Nada de afirmaciones vagas ("Las razones son estructurales"). Nombra la cosa concreta. Nada de extremos perezosos ("todo", "siempre", "nunca", "nadie") haciendo un trabajo que no les toca.

5. **Mete al lector en la escena.** Nada de narrador que observa desde lejos. "Tú" funciona mejor que "la gente". Lo concreto gana a lo abstracto.

6. **Varía el ritmo.** Mezcla frases largas y cortas. Dos elementos funcionan mejor que tres. Cierra cada párrafo de una manera distinta. Nada de rayas largas (—).

7. **Confía en el lector.** Afirma los hechos sin rodeos. Sin suavizar, sin justificarte, sin llevarle de la mano.

8. **Quita las frases de póster.** Si suena a cita para enmarcar o a post motivacional, reescríbela.

9. **No inventes vivencias ajenas.** Si escribes en nombre de otra persona, usa solo las experiencias, datos y opiniones que te ha contado. Nada de anécdotas, cifras, emociones ni aprendizajes de relleno ("Recuerdo mi primer día...", "Me emocioné al ver..."). Si falta material, pregunta o deja un hueco marcado como `[completar]`.

## Comprobaciones rápidas

Antes de entregar un texto:

- ¿Hay adverbios? Quítalos.
- ¿Hay pasivas, con "ser" o con "se"? Busca a quien hace la acción y ponlo de sujeto.
- ¿Una cosa hace algo propio de una persona ("la decisión surge")? Nombra a la persona.
- ¿Alguna frase empieza por Qué, Cómo, Por qué o "Lo que"? Reestructúrala.
- ¿Hay calentamiento tipo "La verdad es que" o "Esto es lo que aprendí"? Ve al grano.
- ¿Hay algún "No es X, es Y" o "No solo X, sino Y"? Di Y.
- ¿Tres frases seguidas miden lo mismo? Rompe una.
- ¿El párrafo acaba con una frase lapidaria? Cambia el cierre.
- ¿Hay alguna raya larga? Quítala.
- ¿Hay una afirmación vaga ("Las implicaciones son enormes")? Nombra la implicación.
- ¿Habla un narrador a distancia ("Nadie diseñó esto")? Pon al lector en la escena.
- ¿Hay metacomentarios ("En el resto del artículo...")? Bórralos y avanza.
- ¿Cierre de LinkedIn, un emoji por línea o más de tres hashtags? Fuera.
- ¿Suena a inglés traducido (Mayúsculas En Cada Palabra, gerundio de posterioridad)? Reescríbelo en español.
- ¿Escribes por otra persona? Comprueba que cada vivencia y cada dato salen de lo que te contó.

## Puntuación

Puntúa de 1 a 10 cada dimensión:

| Dimensión | Pregunta |
|-----------|----------|
| Claridad | ¿Afirma o anuncia? |
| Ritmo | ¿Variado o de metrónomo? |
| Confianza | ¿Respeta la inteligencia del lector? |
| Autenticidad | ¿Suena a una persona? |
| Densidad | ¿Sobra algo? |

Por debajo de 35/50: reescribe.

## Ejemplos

Ver [references/examples.md](references/examples.md) para transformaciones de antes y después.

## Licencia

MIT
