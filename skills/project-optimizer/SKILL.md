---
name: project-optimizer
description: "Optimiza proyectos existentes: mejora arquitectura, reduce deuda técnica, aplica simplificación y performance. Inspirado en mattpocock/skills (improve-codebase-architecture) y addyosmani (code-simplification, performance-optimization). Úsalo en repos existentes cuando el usuario pida optimizar, refactorizar o mejorar calidad."
type: workflow
lifecycle: active
---

# Project Optimizer — Mejorar proyectos existentes

Aplica un proceso estructurado de optimización a codebases existentes. Combina prácticas de:

- mattpocock/skills: improve-codebase-architecture, domain-modeling, diagnosing-bugs
- addyosmani/agent-skills: code-simplification, performance-optimization, code-review

## Workflow

1. **Entender el estado actual**
   - Lee README, estructura de carpetas y archivos de configuración principales.
   - Identifica el dominio (si hay GLOSSARY o similar, úsalo).
   - Detecta puntos de dolor: archivos grandes, dependencias circulares, falta de tests, deuda evidente.

2. **Análisis de arquitectura**
   - Identifica módulos profundos vs superficiales.
   - Busca oportunidades de "deep modules" (interfaz pequeña, implementación compleja bien encapsulada).
   - Genera candidatos de mejora (como el HTML report de improve-codebase-architecture).

3. **Priorizar**
   - Clasifica por impacto / esfuerzo.
   - Propón 3-5 cambios concretos (no más).

4. **Aplicar o proponer cambios**
   - Simplificación: elimina ruido, nombres vagos, over-abstraction (Chesterton's Fence).
   - Performance: mide primero si es posible; si no, identifica hotspots obvios.
   - Tests: asegura que los cambios críticos tengan cobertura o propone tests.
   - ADRs o documentación breve del "por qué" de cambios importantes.

5. **Verificación**
   - Si hay tests, ejecútalos.
   - Revisa que el comportamiento se preserve.
   - Propón un PR o diff claro.

## Cuándo usar
- "Optimiza este proyecto"
- "Mejora la arquitectura de X"
- "Reduce la deuda técnica"
- "Simplifica este código"
- "Revisa y mejora el rendimiento"

## Notas para el usuario (Technical Lead Full Stack)
- Enfócate en backend/TS/Python cuando aplique.
- Mantén compatibilidad con flujos Scrum/agile existentes.
- Prefiere cambios incrementales y verificables.
