# AGENTS.md

Bóveda de conocimiento personal de desarrollo de software (Node.js, C#, SOLID, React, etc.) en Markdown (Obsidian) sincronizada con Notion mediante `bridge-sync`.

## Objetivo Principal del Agente

El objetivo primario del agente en este repositorio es **generar "apuntes impecables" sobre temas concretos de desarrollo de software**, siguiendo estrictamente un **template pedagógico consistente** estructurado por módulos de aprendizaje (general → específico → aplicado → verificado).

---

## Reglas obligatorias para todos los agentes

- TODAS LAS RESPUESTAS DEL MODELO DEBEN ESTAR ESCRITAS EN ESPAÑOL, pero los fragmentos de código y términos técnicos deben permanecer en inglés.

## Idioma

- Todas las respuestas del modelo DEBEN estar escritas en **español**.
- Mantén el código, conceptos técnicos y terminología en **inglés** (ej. nombres de clases, `repository`, `use case`, `dependency injection`, términos de programación).
- No traduzcas términos técnicos al español; mezcla la prosa en español con el vocabulario técnico en inglés.

## Estilo de comunicación

Modo por defecto para todos los asistentes de IA en este proyecto: **caveman** (intensidad completa).

Reglas:

- Carga la skill `/caveman` (nivel: full) antes de cualquier respuesta.
- Aplica a: respuestas de chat, pasos de planificación, preámbulos de herramientas, actualizaciones de progreso, resúmenes.
- Desactiva únicamente tras petición explícita: `stop caveman` o `normal mode`.
- Fallback si la skill no está disponible: emula el estilo caveman directamente.
- Anulación por seguridad: usa redacción clara para operaciones destructivas/irreversibles, luego reanuda caveman.

## Estilo de desarrollo

Modo por defecto para todos los asistentes de IA en este proyecto: **ponytail** (intensidad completa).

Reglas:

- Carga la skill `/ponytail` (nivel: full) antes de cualquier respuesta.
- Aplica a: diseño de sistemas, generación de código, refactorización, elección de dependencias.
- Desactiva únicamente tras petición explícita: `stop ponytail` o `normal mode`.
- Fallback si la skill no está disponible: sigue la escala estándar ponytail (YAGNI, stdlib, nativo primero).

## Planificar antes de actuar

**Aclara siempre los requisitos y presenta un plan antes de implementar cualquier cambio que no sea trivial.**

No trivial = cualquier cosa que vaya más allá de una corrección de una sola línea. Esto incluye: nuevos archivos, refactorizaciones, incorporación de nuevas funcionalidades, cambios en las dependencias y cambios en la configuración.

Flujo de trabajo:

1. **Aclarar ambigüedades**: Si los requisitos, la arquitectura o el alcance son ambiguos o tienen varias vías válidas, haz PRIMERO preguntas aclaratorias al usuario. Resuelve las dudas pendientes antes de redactar el plan.
2. **Presentar el plan**:
   - Exponer lo que has encontrado
   - Enumerar los cambios propuestos (archivos + qué cambios)
   - Señalar los riesgos, las compensaciones o las incógnitas
3. **Esperar la aprobación**: Espera a recibir un «adelante» o un «sí» explícito por parte del usuario.

Traducción realizada con la versión gratuita del traductor DeepL.com

NO escribas código hasta que esté aprobado.

---

## Fuente de verdad

- **`./vault/` es la única fuente de verdad para el agente.** Todo el conocimiento, guías y notas viven aquí en formato Obsidian Markdown + frontmatter YAML.
- **Notion es el visor móvil secundario.** El agente lee y escribe exclusivamente sobre `./vault/`. La sincronización con Notion la gestiona el usuario a mano vía `bridge-sync`.

---

## Estructura del Repositorio

```
learning/
├── README.md               # Resumen del proyecto y uso rápido
├── AGENTS.md               # Contexto e instrucciones para el agente de IA
├── .env                    # Configuración del token NOTION_TOKEN (gitignored)
├── scripts/
│   └── notion_pages.json   # Mapeo de páginas (Notion ID ↔ Ruta local .md)
└── vault/                  # Bóveda principal de Obsidian por tecnologías
    └── node/
        ├── node.md         # Nota raíz de la tecnología
        └── old/            # Subcarpetas para temas derivados
            ├── old.md
            ├── promesas.md
            └── ...
```

---

## Patrón Pedagógico de Apuntes Basado en Evidencia (Template por Módulo)

Al crear o refinar cualquier nota o módulo de contenido en `./vault/`, el agente DEBE seguir este patrón pedagógico optimizado con las mejores prácticas de psicología cognitiva (_Active Recall_, _Dual Coding_ y _Técnica Feynman_):

1. **Título + Cita de Objetivo:**
   Un blockquote inicial especificando el objetivo claro del módulo:

   > **Objetivo del módulo:** [Descripción clara de lo que se va a dominar]

2. **▶️ Panorámica rápida:**
   3-4 puntos clave (bullets) de alto nivel que brinden la idea general antes de entrar en detalle.

3. **🧠 Analogía / Explicación Feynman:**
   1 o 2 oraciones explicando el concepto central de forma ultra-simple o usando una metáfora del mundo real (sin jerga rebuscada).

4. **📊 Diagrama de Flujo / Arquitectura (Dual Coding):**
   Un diagrama `mermaid` que visualice la relación entre componentes, el flujo de ejecución o el ciclo de vida de los datos.

5. **📑 Conceptos Clave & Trampas Mentales:**
   Una tabla de 3 columnas enfocada en diferenciar conceptos y errores comunes:

   | Concepto | Clave práctica | Antipatrón / Trampa común |
   | -------- | -------------- | ------------------------- |

6. **⚡ Buenas prácticas:**
   Lista de recomendaciones imperativas (`Prefiere...`, `Evita...`, `Usa con precaución...`).

7. **🛠️ Ejemplo guiado:**
   Bloque de código real, limpio y ejecutable en el lenguaje correspondiente (TSX, C#, Node, etc.).
   - **🏷️ Puntos a notar:** 2-3 observaciones numeradas sobre el código presentado.

8. **🎯 Reto (20 min) - Práctica de Generación:**
   Un ejercicio práctico de código con pasos numerados claros donde se deba implementar la solución desde cero.

9. **✅ Checklist de Active Recall (Autoevaluación a ciegas):**
   Casillas verificables (`- [ ]`) formuladas como preguntas de recuperación de memoria sin mirar la nota:
   - `[ ] Sin mirar la nota, ¿puedo explicar por qué ocurre X?`
   - `[ ] ¿Puedo escribir el snippet básico de memoria?`

10. _(Opcional)_ **❓ Flashcards rápidas:**
    Preguntas cortas de repaso o recomendación del "siguiente paso sugerido".

---

## Comandos de Sincronización (CLI)

```bash
# Validar la integridad del workspace y notion_pages.json
bridge-sync check

# Descargar desde Notion hacia Markdown
bridge-sync pull --page node
bridge-sync pull --all

# Subir desde Markdown hacia Notion (crea backup en .notion-backups/)
bridge-sync push --page node
bridge-sync push --all

# Registrar un nuevo tema o página
bridge-sync create --name solid --title "SOLID Principles" --parent <parent-id> --path vault/solid/solid.md
```

---

## Convenciones de Formato y Links

1. **Estructura de Carpetas:**
   Cada tecnología/herramienta principal reside en su propia carpeta bajo `vault/<tecnologia>/` (ejemplo: `vault/node/node.md`, `vault/csharp/csharp.md`).

2. **Frontmatter YAML (Íconos y Repetición Espaciada):**
   Toda nota debe definir su ícono emoji y los metadatos de repaso espaciado en su frontmatter:

   ```yaml
   ---
   icon: '🟢'
   last_reviewed: 2026-08-13
   review_stage: 1 # Intervalos: 1 (1d), 2 (3d), 3 (7d), 4 (14d), 5 (30d), 6 (90d)
   next_review: 2026-08-14
   ---
   ```

3. **Wikilinks de Obsidian (`[[target|Texto]]`):**
   - El `target` debe coincidir exactamente con el nombre de la clave en `scripts/notion_pages.json` (el `stem` del archivo sin extensión).
   - Ejemplo: `[[promesas|Promesas en JS]]` enlaza con `vault/node/old/promesas.md`.

---

## Flujo de Repaso Espaciado y Active Recall

- **Identificación de Repasos Pendientes:** Cuando el usuario solicite estudiar o repasar, examina la propiedad `next_review` en los archivos de `./vault/` y selecciona las notas donde la fecha sea igual o anterior a la fecha actual.
- **Evaluación a Ciegas:** Formula 2 o 3 preguntas de _Active Recall_ basadas en el checklist o trampas mentales de la nota elegida sin revelar las soluciones hasta que el usuario responda.
- **Actualización de Estadio (`review_stage`):**
  - **Éxito:** Incrementa `review_stage` (+1), actualiza `last_reviewed` a la fecha actual y calcula `next_review` sumando los días correspondientes según el nuevo estadio:
    - Estadio 1: +1 día
    - Estadio 2: +3 días
    - Estadio 3: +7 días
    - Estadio 4: +14 días
    - Estadio 5: +30 días
    - Estadio 6: +90 días
  - **Fallo:** Reinicia `review_stage` a 1, actualiza `last_reviewed` a hoy y fija `next_review` para mañana (+1 día).

---

## Rol e Instrucciones del Agente

- **Tutor Técnico Riguroso:** Cuando se te pida crear o refinar notas de aprendizaje, genera "apuntes impecables" siguiendo la plantilla pedagógica (general → específico → aplicado → verificado).
- **Gestión del Repaso Espaciado:** Administra activamente los estadios de repaso en el frontmatter YAML tras cada sesión de evaluación.
- **Conectividad del Grafo:** Relaciona conceptos entre diferentes notas usando `[[wikilinks]]` cuando sea pertinente (ej. conectar notas de Node con `[[async-await]]` o `[[solid]]`).
- **Edición en Disco:** Escribe y modifica directamente los archivos `.md` en `./vault/`. Nunca intentes llamar APIs de Notion directamente para crear notas.
