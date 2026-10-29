# Skills briefing

Catálogo para consultar después: qué hace cada skill de Superpowers, Matt Pocock, Addy Osmani y Gentle AI, y qué te cambia en OpenSpecs, ai-mastery-course, LogsKibana y Psicorel.

Preparado para Claude Code, Grok y Antigravity. Una skill es una carpeta con `SKILL.md`. La descripción del YAML es lo que dispara la skill.

## Cómo usarlo

1. Lee [proyectos.md](proyectos.md) para el corte por repo.
2. Lee [plan-30-dias.md](plan-30-dias.md) antes de instalar nada.
3. Copia solo las carpetas de [skills/](skills/) que el plan nombre a `.claude/skills/` del repo, o a `~/.claude/skills/` si las quieres en todas las sesiones de Claude Code.

No instales el catálogo entero. TDD aparece tres veces. Una puerta de entrada, no dos.

## Grok Bot

Este repositorio es la copia consultable. Grok Bot no ve el chat donde se preparó el briefing: lee este repo.

En un chat de Grok Bot:

```text
Instala las skills de https://github.com/jesusprodriguezUnir/skills-briefing.
Lee cada carpeta skills/<nombre>/SKILL.md y cópiala a tu biblioteca de skills
(~/.grok/skills/ o la carpeta de workflows que uses).
No instales el catálogo entero de Superpowers ni de Osmani: solo estas 10.
Al terminar, lista las que quedaron instaladas.
```

Las 10 carpetas están en [skills/](skills/). El resto de este repo es el índice: qué hace cada skill de los repos de origen y en qué proyecto tuyo encaja.

| Agente | Dónde copiar una skill |
|---|---|
| Grok Bot | `~/.grok/skills/<nombre>/` o la carpeta de workflows del bot |
| Claude Code | `.claude/skills/` en el repo, o `~/.claude/skills/` |
| Antigravity | el directorio de skills del proyecto |

## Capítulos

| Capítulo | Skills |
|---|---|
| [Obra · Superpowers](superpowers.md) | 15 |
| [Matt Pocock · Ingeniería](matt-eng.md) | 20 |
| [Matt Pocock · Productividad](matt-prod.md) | 7 |
| [Addy Osmani · Antes de codear](addy-pensar.md) | 9 |
| [Addy Osmani · Mientras construyes](addy-construir.md) | 8 |
| [Addy Osmani · Antes de main](addy-entregar.md) | 8 |
| [Gentle AI · Lo que acabo de añadir](gentle.md) | 11 |
| [Pack propio](propio.md) | 10 |
| [Corte por proyecto](proyectos.md) | |
| [Plan de 30 días](plan-30-dias.md) | |

## Pack propio

Skills escritas para estos repos. No son copias de los repositorios de origen.

- [branch-pr](skills/branch-pr/SKILL.md)
- [chained-pr](skills/chained-pr/SKILL.md)
- [cognitive-doc-design](skills/cognitive-doc-design/SKILL.md)
- [comment-writer](skills/comment-writer/SKILL.md)
- [greenfield-project](skills/greenfield-project/SKILL.md)
- [issue-root-resolution](skills/issue-root-resolution/SKILL.md)
- [multi-repo-analyzer](skills/multi-repo-analyzer/SKILL.md)
- [project-optimizer](skills/project-optimizer/SKILL.md)
- [systemic-issue-triage](skills/systemic-issue-triage/SKILL.md)
- [work-unit-commits](skills/work-unit-commits/SKILL.md)

## Fuentes

- [obra/superpowers](https://github.com/obra/superpowers)
- [mattpocock/skills](https://github.com/mattpocock/skills)
- [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)
- [Gentleman-Programming/gentle-ai](https://github.com/Gentleman-Programming/gentle-ai/tree/main/skills)

Las skills de Gentle AI marcadas como "No la copies" están resumidas en su capítulo y no tienen carpeta aquí. Tres de ellas (`gentle-ai-bench`, `rdd-advisory-transport`, `gentle-ai-collab-perfect`) solo aplican dentro de ese repositorio.
