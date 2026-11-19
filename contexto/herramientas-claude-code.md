# Herramientas de Claude Code

- **Archivos y código.** Puedo leer, crear y editar archivos (texto, código, notebooks Jupyter, imágenes y PDF en lectura), y buscar por nombre o contenido en todo el clon.
- **Terminal en Windows.** Ejecuto comandos en PowerShell 5.1 y en Git Bash: Git, CLI de GitHub (`gh`), y los lenguajes o herramientas que estén instalados en el PC. Puedo dejar procesos largos corriendo en segundo plano.
- **Subagentes y orquestación.** Puedo lanzar subagentes para trabajo en paralelo (exploración de código, planificación, tareas generales) y aislar cambios en un `git worktree` propio.
- **Web.** Puedo hacer búsquedas web y leer páginas públicas. No accedo a contenido privado o autenticado salvo por herramientas con sesión (por ejemplo `gh`).
- **Tareas programadas.** Puedo repetir una tarea a intervalos (`/loop`), programar recordatorios o agentes en la nube y enviar notificaciones.
- **Revisión.** Tengo comandos para revisar cambios en busca de errores, simplificar código y hacer revisiones de seguridad.
- **Memoria propia.** Guardo memoria persistente local entre sesiones, aparte de este repositorio.
- **Restricciones.** Opero bajo un modo de permisos elegido por Matías: algunos comandos (por ejemplo `git pull`, `git push` o comandos encadenados) pueden requerir su aprobación. No tengo conectores MCP de aplicaciones de escritorio ni de servicios como Drive o Gmail configurados en esta sesión.
