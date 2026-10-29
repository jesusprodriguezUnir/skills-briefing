---
name: chained-pr
description: "Parte un cambio que supera las 400 líneas en pull requests encadenadas y revisables. Úsala cuando un diff no cabe en una review o el trabajo tiene dependencias entre trozos."
type: workflow
lifecycle: active
---

# Pull requests encadenadas

1. Estima líneas cambiadas y lista unidades que se pueden entregar solas.
2. Si cada trozo puede entrar en la rama por defecto por separado, apílalos: cada PR apunta a main y el siguiente espera al anterior.
3. Si el conjunto solo integra junto, abre un tracker en draft y encadena: el primer hijo apunta al tracker y cada hijo siguiente apunta a su padre.
4. En cada PR escribe inicio, fin, de qué depende, qué queda después y qué está fuera. Marca el PR actual en un diagrama corto.
5. No mezcles estrategias a mitad. No metas en un hijo el diff del padre.
6. El tracker no se mergea hasta que los hijos están revisados.

## Hecho cuando
- Cada PR se entiende en menos de una hora.
- El diff de cada una muestra solo su unidad.
- Hay orden, dependencia y plan de verificación.
