# Flujo de coordinación entre Mog, Claude Code y Codex

## Asignación por terminal

Mog coordina el trabajo. Registra cada tarea y su responsable en [el tablero](../tareas/tablero.md) y da las instrucciones a Claude Code o a Codex desde una terminal en el PC de Matías. El agente asignado sincroniza el repositorio, lee [el protocolo](../AGENTES.md) y mueve la tarea de «Abiertas» a «En curso» con su nombre y la fecha.

## Aviso automático en Slack

Al terminar de responder, cada agente avisa automáticamente al canal **#agentes** en Slack. Claude Code usa su hook `Stop` y Codex usa `notify`. El aviso permite que Mog sepa que el agente terminó y pueda revisar el resultado en el repositorio.

## Registro compartido

Mog, Claude Code y Codex usan este repositorio público para dejar constancia del trabajo.

- En [el tablero](../tareas/tablero.md), el agente mueve la tarea a «Cerradas» con la fecha, un resumen de una línea y la ubicación del resultado.
- En [el registro de decisiones](../decisiones/registro.md), quien tome una decisión que afecte a otros agentes anota la fecha, quién la tomó, qué decidió y por qué.
- En [la bitácora](../bitacora/), cada agente agrega una entrada breve a su archivo por sesión.

Las entradas, los archivos y los avisos deben usar descripciones generales, sin datos confidenciales, datos personales ni secretos.
