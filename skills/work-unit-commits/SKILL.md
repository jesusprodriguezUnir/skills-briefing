---
name: work-unit-commits
description: "Haz commits por unidad de comportamiento, con su test y su doc. Úsala al implementar, al partir una rama o cuando los tests se quedan en un commit aparte."
type: workflow
lifecycle: active
---

# Commits por unidad de trabajo

1. Un commit es un comportamiento, un fix o un doc que se entiende solo. No un tipo de archivo.
2. El test viaja en el mismo commit que el comportamiento que verifica.
3. El doc de cara al usuario viaja con el cambio que explica.
4. El mensaje dice el resultado, en conventional commit. No listes archivos.
5. Después de ese commit, el repo sigue teniendo sentido. Se puede revertir sin llevarse trabajo ajeno.
6. Si la suma se acerca a 400 líneas, promociona grupos de commits a chained-pr antes de seguir.

## Hecho cuando
- Hay un propósito por commit.
- El comando de test de esa unidad está anotado con su resultado, o un N/A explícito si no hay frontera de runtime.
