# Addy Osmani · Antes de main

Review, seguridad, observabilidad y el día del deploy.

Lo que un technical lead no debería dejar en el prompt del momento. Son contratos de salida.

Fuente: [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)

| Skill | Marca | Qué hace | En tus proyectos |
|---|---|---|---|
| `code-review-and-quality` | Quédate con el principio | Review en varios ejes antes de que el cambio entre en main. | Complementa el review de Pocock. Si ya usas el de dos ejes (estándar + spec), esta sobra. |
| `security-and-hardening` | Instálala | Revisa input, auth, almacenamiento e integraciones contra el OWASP Top 10. | Cualquier login o endpoint nuevo de OpenSpecs pasa por aquí antes del merge. |
| `observability-and-instrumentation` | Instálala | Añade logs, métricas y trazas para que producción se pueda diagnosticar. | LogsKibana predica observabilidad. Esta skill exige que tus propios servicios también la tengan. |
| `ci-cd-and-automation` | Instálala | Deja quality gates, tests y estrategia de deploy en el pipeline. | Los repos activos dejan de depender de que te acuerdes de lanzar la suite. |
| `git-workflow-and-versioning` | Instálala | Ramas, commits atómicos, conflictos y PRs con un flujo explícito. | Encaja con work-unit-commits de Gentle AI. Usa las dos juntas: esta es el marco, aquella es el corte. |
| `documentation-and-adrs` | Instálala | Registra la decisión de arquitectura en el momento en que se toma. | El curso y OpenSpecs acumulan ADRs cortos en vez de un README que miente. |
| `deprecation-and-migration` | Quédate con el principio | Retira APIs y columnas con expand/contract, sin downtime de manual. | Cuando OpenSpecs cambie un contrato, los consumidores no se enteran el día del corte. |
| `shipping-and-launch` | Instálala | Checklist de salida: monitorización, rollout por fases y rollback. | Un deploy de LogsKibana o de OpenSpecs tiene marcha atrás escrita antes de pulsar. |
