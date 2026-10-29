# Gentle AI · Lo que acabo de añadir

PRs pequeñas, un arreglo por raíz, y docs que se pueden revisar.

Once skills. Varias están atadas al CI de ese repo (Go, bench, RDD). De esas me quedo con el principio y no las copio a tus proyectos. Las transferibles ya están escritas como skills propias, en español, listas para Claude Code.

Fuente: [Gentleman-Programming/gentle-ai](https://github.com/Gentleman-Programming/gentle-ai/tree/main/skills)

| Skill | Marca | Qué hace | En tus proyectos |
|---|---|---|---|
| `branch-pr` | Instálala | Abre la rama y el PR con issue enlazado, un solo tipo, y un tope de 400 líneas cambiadas. | Tus PRs de OpenSpecs dejan de mezclar feature, refactor y formato. Skill adaptada: branch-pr. |
| `chained-pr` | Instálala | Si el cambio pasa de 400 líneas, lo parte en PRs apiladas o en una cadena con tracker. | Un rediseño de OpenSpecs se revisa en menos de una hora por trozo, no en un diff de 2.000 líneas. |
| `work-unit-commits` | Instálala | El commit es una unidad de comportamiento. El test y el doc viajan con ella, no en un commit “tests” al final. | Puedes revertir un fix de LogsKibana sin llevarte el refactor de al lado. |
| `systemic-issue-triage` | Instálala | Clasifica por clase de raíz. Dos issues del mismo fallo son un arreglo, no dos parches. Prefiere borrar maquinaria. | El backlog de tus repos activos se encoge en vez de ganar flags, estados y verbos nuevos. |
| `issue-root-resolution` | Instálala | Audita un clúster, demuestra la causa y cierra issues con un test nombrado, no con un “ya debería estar”. | Dejas de cerrar bugs de LogsKibana porque el síntoma desapareció en tu máquina. |
| `cognitive-doc-design` | Instálala | Escribe la decisión primero, el camino feliz después, y el detalle en tablas. Nada de prosa que hay que memorizar. | Las lecciones MDX del curso y los README de los 76 repos se pueden escanear en una review. |
| `comment-writer` | Instálala | Comentarios de review cortos, cálidos y con el porqué. Un punto alto, no diez nits. | Las reviews que dejas en PRs de equipo, y el feedback del curso, se leen en veinte segundos. |
| `rdd-defect-workflow` | Quédate con el principio | Flujo de defecto del propio Gentle AI: reproducir en main, un invariante por PR, worktree, tope de 400, prueba de journey. | Quédate con eso. No instales la maquinaria RDD: es de su runtime, no de tus repos. |
| `gentle-ai-bench` | Quédate con el principio | Un test del corpus no ejecuta el journey. La prueba es el binario real contra el harness. | En LogsKibana: un test que parsea YAML no demuestra que el pipeline indexa. No copies la skill; copia la regla. |
| `rdd-advisory-transport` | No la copies | Un solo contrato Go para que Claude, Codex u OpenCode invoquen al revisor. El adapter solo transporta bytes. | No la instales. Si algún día unificas reviewers entre Claude y Antigravity, el principio es: un contrato, adapters tontos. |
| `gentle-ai-collab-perfect` | No la copies | Protocolo para contribuir a Gentleman-Programming/gentle-ai como externo: issue primero, cuerpo de PR honesto, alcance de contributor. | No va en tus repos. Ábrela solo el día que abras un PR contra gentle-ai. |
