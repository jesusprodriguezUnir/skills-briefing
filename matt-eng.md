# Matt Pocock · Ingeniería

Del issue al módulo profundo, con vocabulario de dominio.

El pack de ingeniería. La pieza que más te cambia el día es el recorrido issue → spec → tickets → implementación, más el informe de arquitectura.

Fuente: [mattpocock/skills](https://github.com/mattpocock/skills)

| Skill | Marca | Qué hace | En tus proyectos |
|---|---|---|---|
| `setup-matt-pocock-skills` | Instálala | Configura una vez el tracker, las etiquetas de triage y dónde viven glosario y ADRs. | Sin esto, el resto del pack no sabe dónde publicar specs. Úsalo en OpenSpecs, no en los 76 repos a la vez. |
| `ask-matt` | Quédate con el principio | Enruta: te dice qué skill del pack encaja con lo que estás haciendo. | Evita cargar TDD cuando lo que toca es un triage, o al revés. |
| `triage` | Instálala | Mueve issues y PRs externas por estados: clasificar, verificar, interrogar y dejar un brief para el agente. | El backlog de OpenSpecs deja de ser una lista y pasa a ser trabajo que un agente puede coger sin preguntarte otra vez. |
| `wayfinder` | Instálala | Parte un bloque enorme en un mapa de decisiones en el tracker y las resuelve de una en una. | Una reescritura de OpenSpecs que no cabe en una sesión deja de perderse al cerrar el chat. |
| `to-spec` | Instálala | Sintetiza la conversación ya hecha en un spec y lo publica. No vuelve a entrevistarte. | Lo que acordaste en Grok o Claude queda escrito antes de que otro agente lo implemente. |
| `to-tickets` | Instálala | Rompe el spec en tickets tracer-bullet, cada uno con sus bloqueos. | Puedes asignar un ticket a Claude y otro a Antigravity sin que se solapen. |
| `implement` | Instálala | Implementa a partir de un spec o de un conjunto de tickets. | El agente construye lo pedido, no lo que infiere del último mensaje. |
| `implement-spec` | Instálala | Implementa el resultado concreto de to-spec y to-tickets. | Cierra el circuito en OpenSpecs: de la conversación al código, sin saltos. |
| `tdd` | Quédate con el principio | Red, green, refactor, con tests de integración cuando el usuario lo pide. | Misma disciplina que Superpowers, con el vocabulario de este pack. Elige una, no las dos a la vez. |
| `domain-modeling` | Instálala | Afila el lenguaje del proyecto: glosario y ADRs, no solo nombres de carpetas. | OpenSpecs y el curso dejan de usar “spec”, “skill” y “plan” para tres cosas distintas. |
| `grill-with-docs` | Instálala | Entrevista dura del diseño y, de paso, escribe el ADR y el glosario. | Una decisión de arquitectura de OpenSpecs queda registrada, no solo en el chat. |
| `codebase-design` | Instálala | Vocabulario de módulos profundos: interfaz pequeña, implementación escondida, costuras testeables. | Te da el criterio para partir un módulo de TypeScript antes de pedirle al agente que lo haga. |
| `improve-codebase-architecture` | Instálala | Escanea el repo, saca un informe HTML de oportunidades de profundidad y te interroga sobre la que elijas. | Es el análisis de arquitectura que pedías para un repo concreto, no un consejo genérico. |
| `diagnosing-bugs` | Instálala | Bucle de diagnóstico para bugs duros y regresiones de rendimiento. | LogsKibana: primero la medida o la reproducción, después el parche. |
| `prototype` | Quédate con el principio | Hace un prototipo desechable para responder una pregunta de estado o de UI. | Psicorel o una pantalla nueva se prueban sin comprometer la arquitectura. |
| `research` | Instálala | Investiga contra fuentes primarias y deja el hallazgo en un Markdown del repo. | Una duda de API de Kibana o de un SDK queda citada en el repo, no en un chat que se pierde. |
| `code-review` | Instálala | Revisa el diff en dos ejes a la vez: estándares del repo y fidelidad al spec. | Un PR de agente se rechaza si el código está limpio pero no hace lo que el ticket pedía. |
| `pr` | Instálala | Escribe el cuerpo del pull request. | Los PRs de los repos activos cuentan el porqué, no el listado de archivos. |
| `retro` | Quédate con el principio | Retrospectiva de la sesión de código. | Útil al cerrar un sprint corto contigo mismo. No la cargues en cada commit. |
| `wizard` | Quédate con el principio | Genera un asistente bash para los pasos que solo puedes hacer tú: secretos, dashboards, cutovers. | El alta de un índice de Kibana o un secreto de CI no se le delega al agente a ciegas. |
