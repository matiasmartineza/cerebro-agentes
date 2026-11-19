# Cerebro Colectivo

Espacio compartido donde **Mog**, **Claude Code** y **Codex CLI** registran contexto, decisiones y estado de tareas para coordinarse entre agentes. Matías es el dueño y tiene la última palabra.

> Este repositorio es **público**. No escribir aquí datos confidenciales del trabajo (clientes, planos, correos, contraseñas, RUT ni datos personales). Usar descripciones generales o referencias internas.

## Propósito

Tener un solo lugar de verdad para que cualquier agente, local o en la nube, pueda saber qué se está haciendo, qué se decidió y retomar el trabajo de otro sin depender de una conversación en particular.

- **Mog**: coordinador. Reparte tareas, revisa resultados y mantiene este repositorio ordenado.
- **Claude Code** y **Codex**: ejecutores, tanto sus versiones locales en el PC de Matías como sus sesiones en la nube.

## Cómo usarlo

Cada agente lee `AGENTES.md` antes de empezar y luego escribe sus notas en archivos o issues:

- `tareas/tablero.md`: tareas abiertas, en curso y cerradas, con su responsable. También se pueden usar issues de GitHub para pedidos puntuales entre agentes.
- `decisiones/registro.md`: decisiones tomadas, con fecha y motivo.
- `contexto/`: conocimiento estable, como las herramientas de cada agente (`herramientas-<agente>.md`).
- `bitacora/<agente>.md`: notas breves de lo que hizo cada agente en cada sesión.

## Estado actual

- 2026-11-19: repositorio creado con su estructura inicial y protocolo.
- Codex (local): conectado; documentó sus herramientas y su bitácora.
- Claude Code (local): pendiente de iniciar sesión en la versión de comandos.