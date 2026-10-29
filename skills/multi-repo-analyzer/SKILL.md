---
name: multi-repo-analyzer
description: "Analiza múltiples repositorios GitHub del usuario (estructura, arquitectura, deuda técnica, tech stack) usando enfoques tipo Graphify y Repomix. Úsalo cuando el usuario pida revisar, mapear o generar un informe de todos sus proyectos o de un conjunto de repos."
type: workflow
lifecycle: active
---

# Multi-Repo Analyzer — Visión global de todos tus proyectos

Usa este skill cuando necesites analizar, mapear o generar un informe de varios repositorios a la vez (especialmente los ~76 del usuario jesusprodriguezUnir o cualquier conjunto).

Combina ideas de Graphify (knowledge graph) y Repomix (empaquetado AI-friendly).

## Workflow

1. **Listar repositorios**
   - Si tienes acceso a GitHub (gh CLI o API), lista repos del usuario: `gh repo list jesusprodriguezUnir --limit 100 --json name,description,language,updatedAt,url`
   - O pide al usuario la lista de URLs / paths locales.

2. **Para cada repo (o los prioritarios)**
   - Clona o usa path local si ya está.
   - Genera estructura: `tree -L 3 -I 'node_modules|.git|dist|build|__pycache__|.venv'` o equivalente.
   - Detecta tech stack: busca package.json, pyproject.toml, requirements.txt, go.mod, Cargo.toml, Dockerfile, etc.
   - Extrae métricas básicas: líneas de código (si tienes cloc), número de archivos, últimos commits.
   - Si es posible, ejecuta o simula un análisis tipo Graphify: identifica módulos principales, dependencias cruzadas, puntos de entrada.

3. **Empaquetar para análisis profundo (opcional)**
   - Usa Repomix si está disponible: `npx repomix --remote owner/repo` o en local.
   - O genera un resumen compacto en Markdown.

4. **Generar informe consolidado**
   - Tabla resumen: Repo | Lenguaje principal | Stack detectado | Última actividad | Estado (activo/abandonado) | Notas de arquitectura.
   - Sección de patrones comunes y deuda técnica recurrente.
   - Recomendaciones prioritarias (top 3-5 mejoras).
   - Si aplica, sugiere skills específicas de optimización o greenfield.

5. **Salida**
   - Entrega un Markdown claro, preferiblemente con tablas.
   - Guarda el informe en un archivo si el usuario lo pide (ej. `analisis-repos.md`).

## Cuándo usar
- "Analiza todos mis proyectos"
- "Dame un overview de mis repos"
- "Qué deuda técnica tengo en mis proyectos"
- "Mapea la arquitectura de mis repositorios"

## Notas
- Prioriza repos actualizados recientemente.
- Sé conciso: el usuario es Technical Lead, no necesita explicaciones básicas.
- Si un repo es privado y no hay acceso, indícalo y continúa con los públicos.
