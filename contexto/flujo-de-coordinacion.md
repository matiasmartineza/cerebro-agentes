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

## Tareas para Claude Code: Session Launcher

Desde el 2026-11-19, Mog no abre sesiones nuevas de Claude Code por su cuenta, porque no aparecen en la app de Matías. Toda tarea se escribe en la sesión existente **Session Launcher**, que abre una sesión nueva para cada tarea, visible en la app y con contexto limpio. El mensaje debe entrar por la sesión abierta en la app de escritorio: si se retoma la sesión desde la terminal, Session Launcher no puede abrir sesiones.

Formato del mensaje (todos los campos son obligatorios):

```
TAREA PARA LANZAR
Carpeta: <ruta absoluta donde debe trabajar>
Modelo: <claude-opus-5-5 | claude-sonnet-5-5 | claude-haiku-5-5>
Razonamiento: <low | medium | high>
Tarea: <qué hacer, completa y autocontenida>
Terminado cuando: <criterio concreto>
```

Elección de modelo y razonamiento:

- Haiku con low para tareas simples y mecánicas.
- Sonnet con medium para el trabajo normal.
- Opus con high para tareas complejas o delicadas. Es el máximo.
- Si no está claro cuál usar, Mog le pregunta a Matías antes de enviar la tarea.

La sesión nueva no ve conversaciones anteriores, así que la tarea debe ser autocontenida. Al terminar, el aviso automático llega a #agentes, como siempre.
## Tareas para Codex: desde la app

Desde el 2026-11-19, Mog no lanza Codex por terminal. Las sesiones nuevas se crean en la app de escritorio (ChatGPT/Codex). Mog abre un chat nuevo, entra en la pestaña «Work», elige el proyecto, que fija la carpeta, revisa el modelo y el razonamiento, y pega la tarea autocontenida. Para continuar un trabajo, escribe en el chat que ya existe. Así cada sesión queda visible en la app. El proyecto «cerebro-agentes» ya está creado.