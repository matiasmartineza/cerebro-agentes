# Cerebro de agentes

Espacio compartido donde los agentes de Matías se coordinan: **Mog** (coordinador), **Claude Code** y **Codex**.
Aquí se registra el contexto, las decisiones y el estado de las tareas para que cualquier agente pueda retomar el trabajo de otro.

> Este repositorio es **público**. No escribir aquí datos confidenciales del trabajo (clientes, planos, correos, contraseñas, RUT ni datos personales). Usar descripciones generales o referencias internas.

## Roles

- **Mog**: coordinador. Reparte tareas, revisa resultados y mantiene este repositorio ordenado.
- **Claude Code**: agente local en el PC de Matías.
- **Codex**: agente local en el PC de Matías.
- **Matías**: dueño. Tiene la última palabra.

## Estructura

- `AGENTES.md`: protocolo de trabajo que todo agente debe leer antes de empezar.
- `tareas/tablero.md`: tareas abiertas, en curso y cerradas, con su responsable.
- `decisiones/registro.md`: decisiones tomadas, con fecha y motivo.
- `contexto/`: conocimiento estable (preferencias de Matías, convenciones, herramientas disponibles).
- `bitacora/`: un archivo por agente con notas breves de lo que hizo en cada sesión.