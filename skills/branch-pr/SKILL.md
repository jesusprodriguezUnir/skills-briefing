---
name: branch-pr
description: "Abre ramas y pull requests pequeñas: un tipo, issue enlazado y tope de 400 líneas. Úsala al crear una rama, preparar un PR o revisar si un diff cabe en una review."
type: workflow
lifecycle: active
---

# Rama y pull request

1. Nombra la rama `tipo/descripcion-corta` en minúsculas: feat, fix, chore, docs, refactor, perf, test, ci.
2. Enlaza un issue. `Closes #N` si el merge lo cierra. `Refs #N` si no. No mezcles las dos para el mismo issue.
3. Un solo tipo de cambio por PR. Si hay feature y refactor, son dos PRs.
4. Cuenta líneas añadidas más borradas. Por encima de 400, para y usa chained-pr.
5. El cuerpo del PR dice qué cambia, por qué, cómo se probó y qué queda fuera.
6. No atribuyas el commit a un agente. No hagas force-push a la rama por defecto.

## Hecho cuando
- La rama cumple el patrón.
- El PR enlaza un issue y declara un solo tipo.
- El diff cabe en una review o ya está partido.
