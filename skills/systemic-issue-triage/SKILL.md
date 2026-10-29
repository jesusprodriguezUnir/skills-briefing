---
name: systemic-issue-triage
description: "Triagea bugs por clase de raíz y arregla el clúster, no el síntoma. Úsala con un backlog, una avalancha de issues o antes de diseñar un fix."
type: workflow
lifecycle: active
---

# Triage por raíz

Clasifica cada issue en un solo cubo antes de tocar código:

| Cubo | Qué es | Qué haces |
|---|---|---|
| A | Lo tapa un cambio que ya está en vuelo | Nombras el cambio y el test que lo demostrará |
| B | Duplicado de una clase conocida | Apuntas al tracker canónico |
| C | Bug nuevo | Entra en un clúster, nunca en un parche suelto |
| D | Feature | No se disfraza de bug |
| E | No se entiende | Preguntas. No adivinas |

Reglas:

1. Dos issues con la misma raíz son un arreglo que cierra los dos, con un test nombrado.
2. Antes de añadir un estado, un flag o un verbo nuevo, pregunta qué se puede borrar.
3. Un callejón sin salida se arregla con una salida ejecutable, no con más maquinaria.
4. El texto del issue es una hipótesis. Reproduce el síntoma. Si un test escrito contra el mecanismo que describe pasa en main sin cambios, el diagnóstico está mal y el reporte no.
5. No cierres un hilo que mezcla dos fallos hasta decir cuál se arregló y cuál sigue.

## Hecho cuando
- Hay cubo, raíz y evidencia por issue.
- El arreglo propuesto reduce líneas o estados, o justifica por qué no puede.
