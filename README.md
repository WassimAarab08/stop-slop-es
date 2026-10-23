# Stop Slop en español

Adaptación al español de [stop-slop](https://github.com/hardikpandya/stop-slop), de Hardik Pandya.

Esta skill le enseña a Claude, o a cualquier otro modelo, a detectar y quitar las marcas de la escritura generada por IA cuando escribe en español. Es gratuita y usa la misma licencia MIT que el original.

## Para qué sirve

Los modelos de lenguaje repiten frases, estructuras y ritmos. En español abren correos con "Espero que este mensaje te encuentre bien", cierran posts con "Te leo en comentarios" y meten un "No es X, es Y" en cuanto pueden. Con la skill cargada, el modelo revisa el borrador contra una lista de esos patrones y lo reescribe antes de entregártelo.

## Estructura

```
stop-slop-es/
├── SKILL.md              # Instrucciones principales
├── references/
│   ├── phrases.md        # Frases que hay que quitar
│   ├── structures.md     # Estructuras que hay que evitar
│   └── examples.md       # Ejemplos de antes y después
├── README.md
├── CHANGELOG.md
└── LICENSE
```

## Instalación en Claude Code

Clona el repositorio en tu carpeta de skills personales:

```bash
git clone https://github.com/WassimAarab08/stop-slop-es.git ~/.claude/skills/stop-slop-es
```

En Windows la carpeta está en `%USERPROFILE%\.claude\skills\`. Para usarla en un solo proyecto, clónala en `.claude/skills/stop-slop-es` dentro de ese proyecto.

Claude Code la detecta en la siguiente sesión. Puedes invocarla con `/stop-slop-es` o dejar que Claude la cargue cuando le pidas redactar o revisar un texto.

## Uso en Claude Projects y en otras IA

**Claude Projects:** sube `SKILL.md` y los tres archivos de `references/` al conocimiento del proyecto.

**ChatGPT, Gemini y otros asistentes:** pega las reglas de `SKILL.md` en las instrucciones personalizadas o en las instrucciones de tu GPT o Gem. Si el asistente acepta archivos, adjunta también los de `references/`.

**API:** pon `SKILL.md` en el prompt de sistema y añade los archivos de `references/` cuando los necesites.

## Cambios respecto al original

La adaptación conserva las reglas generales de Hardik Pandya: voz activa, nada de rayas largas, concreción, ritmo variado y la puntuación sobre 50. Por debajo de 35, toca reescribir.

Las diferencias:

- Las listas de frases no son traducciones. Recogen las fórmulas que la IA usa en español: "La verdad es que", "poner en valor", "básicamente", "Quedo a tu entera disposición".
- `phrases.md` tiene dos secciones nuevas: cierres de LinkedIn y fórmulas de correo.
- La regla de la pasiva incluye la pasiva con "se" ("se tomó la decisión"), que esconde al responsable igual que la de "ser".
- Las frases que empiezan por "Lo que..." cuentan como arranques con interrogativo, el equivalente español del arranque en Wh-.
- `structures.md` añade una sección de calcos del inglés, como las mayúsculas en cada palabra de un título o el gerundio de posterioridad.
- Los ejemplos son nuevos: un post de LinkedIn, un correo de trabajo y un mensaje de Slack, cada uno con su antes y su después.
- Hay una regla nueva: si escribes en nombre de otra persona, no inventes experiencias que no te ha contado.
- La skill se llama `stop-slop-es`, así puedes tener instaladas la original y esta sin conflicto de nombres.

## Créditos

Hardik Pandya ([hvpandya.com](https://hvpandya.com)) creó la skill original: la idea, la estructura y las reglas base. [Wassim Aarab](https://github.com/WassimAarab08) la adaptó al español.

## Licencia

MIT, como el original. El archivo [LICENSE](LICENSE) mantiene el copyright de Hardik Pandya y añade el de la adaptación.
