---
name: greenfield-project
description: "Crea proyectos desde cero con metodología estructurada: brainstorming, spec, plan, TDD e implementación incremental. Inspirado en Superpowers y addyosmani agent-skills. Úsalo cuando el usuario quiera empezar un proyecto nuevo o construir una feature grande desde cero."
type: workflow
lifecycle: active
---

# Greenfield Project — Crear desde cero con disciplina

Workflow para construir proyectos o features nuevas de forma confiable. Basado en:

- obra/superpowers: brainstorming → writing-plans → executing-plans / subagent-driven-development + TDD
- addyosmani/agent-skills: /spec → /plan → /build → /test

## Workflow

1. **Clarificar intención (Brainstorming)**
   - Haz preguntas para entender el problema real, usuarios, constraints y éxito.
   - No escribas código todavía.
   - Produce un diseño de alto nivel o PRD breve.

2. **Spec**
   - Escribe un spec claro: objetivos, estructura de carpetas propuesta, stack, criterios de aceptación, qué NO hacer (YAGNI).
   - Guarda en SPEC.md o similar.

3. **Plan**
   - Descompón en tareas pequeñas, verificables y con dependencias.
   - Cada tarea debe poder implementarse y testearse de forma independiente cuando sea posible.
   - Usa worktrees de git si el entorno lo permite para aislar.

4. **Implementación incremental + TDD**
   - Para cada tarea: RED → GREEN → REFACTOR.
   - Implementa el slice más delgado que aporte valor.
   - Commit atómico por tarea completada.
   - Code review ligero al final de cada slice importante.

5. **Cierre**
   - Verifica que los criterios de aceptación se cumplen.
   - Documenta decisiones importantes (ADR breve si aplica).
   - Propón próximos pasos o handoff.

## Cuándo usar
- "Crea un proyecto desde cero"
- "Empieza un nuevo repo con esta idea"
- "Construye esta feature grande siguiendo un plan"
- "Usa una metodología estructurada para este greenfield"

## Notas
- Adaptado a Claude Code, Grok y Antigravity.
- El usuario es Technical Lead: asume conocimiento de Scrum y full-stack; enfócate en estructura y calidad.
- Prefiere TypeScript o Python según el contexto del proyecto.
