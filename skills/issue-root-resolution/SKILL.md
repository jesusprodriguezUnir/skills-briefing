---
name: issue-root-resolution
description: "Cierra un clúster de issues solo con la causa reproducida y un test que la fija. Úsala al auditar raíces, al proponer el fix de un grupo o al dar issues por resueltos."
type: workflow
lifecycle: active
---

# Resolver por la raíz

1. Agrupa por causa, no por título. Una causa, una línea de PR, un rollback.
2. Reproduce el síntoma en la rama por defecto, en limpio. Si no se reproduce, no implementes.
3. Escribe el test que falla con el síntoma, no con el mecanismo que supone el issue.
4. El fix más pequeño que pone el test en verde. Si el forecast pasa de 400 líneas, encadena antes de editar.
5. Cierra cada issue citando el test y el comando. Un "debería estar arreglado" no cierra nada.
6. Si el issue mezcla dos fallos, no lo cierres: di cuál salió y cuál sigue.

## Hecho cuando
- La causa está nombrada y reproducida.
- El test falla antes del fix y pasa después, en el escenario original.
- Cada issue del clúster dice qué prueba lo cierra.
