# Obra · Superpowers

El agente no improvisa: diseña, prueba y demuestra.

Quince skills de proceso. El valor no es una herramienta nueva: es que Claude Code deje de saltarse el diseño, los tests y la prueba de que terminó.

Fuente: [obra/superpowers](https://github.com/obra/superpowers)

| Skill | Marca | Qué hace | En tus proyectos |
|---|---|---|---|
| `using-superpowers` | Instálala | Al abrir sesión, elige la skill antes de responder, incluso antes de preguntar. | En un día con varios repos abiertos, el agente entra en modo análisis, debug o implementación y no mezcla los tres. |
| `brainstorming` | Instálala | Obliga a cerrar el diseño antes de crear una feature, un componente o un cambio de comportamiento. | Las lecciones nuevas de ai-mastery-course y las features de OpenSpecs dejan de nacer como un archivo suelto. |
| `writing-plans` | Instálala | Convierte un spec en un plan de pasos antes de tocar código. | Un cambio que cruza TypeScript y tests se parte en trozos que caben en una sesión. |
| `executing-plans` | Instálala | Ejecuta ese plan en la sesión actual, paso a paso, cuando no hay subagentes. | Sirve en Grok o Antigravity cuando quieres implementación controlada, no un agente suelto. |
| `subagent-driven-development` | Instálala | Reparte tareas independientes del plan entre subagentes, cada uno con su contexto. | Un refactor grande de OpenSpecs no mezcla la API, la UI y los tests en el mismo hilo. |
| `dispatching-parallel-agents` | Quédate con el principio | Lanza trabajo en paralelo solo si no comparten estado ni orden. | Documentación del curso y un fix de LogsKibana pueden ir a la vez, porque no se pisan. |
| `test-driven-development` | Instálala | Escribe el test que falla antes del código, en features y en bugs. | La lógica de OpenSpecs y los parsers de LogsKibana dejan de arreglarse a ojo. |
| `systematic-debugging` | Instálala | Ante un fallo, busca la causa antes de proponer el parche. | Un pipeline de logs que “a veces no indexa” no se tapa con otro if. |
| `using-git-worktrees` | Instálala | Aísla cada feature en un worktree para no ensuciar el árbol de trabajo. | Con ~76 repos, un agente puede estar en una rama sin bloquear la que estás revisando tú. |
| `requesting-code-review` | Instálala | Pide review al cerrar una tarea o antes de mergear, contra el spec. | Dejas de ser el único filtro entre el agente y main. |
| `receiving-code-review` | Instálala | Verifica el comentario de review antes de aplicarlo. No asiente por inercia. | Un review de Antigravity sobre código de Claude no se acepta si no cuadra con el spec. |
| `verification-before-completion` | Instálala | Prohíbe decir “listo” sin el comando y la salida que lo demuestran. | Menos PRs de OpenSpecs o del curso que dicen que pasan y no se ejecutaron. |
| `finishing-a-development-branch` | Quédate con el principio | Cuando los tests pasan, decide merge, PR o limpieza de la rama. | Cierra el trabajo en vez de dejar ramas a medias en el monorepo del día. |
| `writing-skills` | Instálala | Crea, edita y comprueba skills antes de darlas por desplegadas. | Tus convenciones de lead (rama, review, definición de hecho) se vuelven skills, no un mensaje que se olvida. |
| `diagnosing-superpowers` | Quédate con el principio | Postmortem cuando una sesión repitió trabajo, ignoró el plan o se fue de tokens. | Afinas el flujo en vez de echarle la culpa al modelo la próxima vez. |
