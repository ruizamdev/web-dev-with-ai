# Desarrollo web asistido por IA

Plantilla genérica para definir una aplicación y desarrollarla por entregas con agentes de IA y decisiones humanas. No presupone tecnologías ni requisitos de negocio.

## Copiar y adaptar

1. Copia este directorio a un repositorio nuevo o sube su contenido a GitHub. Si habilitas la opción **Template repository** en la configuración de GitHub, podrás reutilizarlo con **Use this template**.
2. Sustituye los campos `[por completar]` con información del proyecto. Un campo vacío o un ejemplo no es una decisión aprobada. Usa «No aplica» con justificación cuando corresponda.
3. Define primero el problema y los requerimientos; después arquitectura, entidades, sistema de diseño y plan de desarrollo, en ese orden. Aún no construyas la aplicación ni su base de datos.
4. La persona responsable revisa y aprueba cada documento antes de avanzar al siguiente. Registra nombre, fecha y versión exacta en su tabla de decisiones.
5. Prepara E001 con el planificador, aprueba su alcance y ejecuta el flujo de entregas. Para E002 y siguientes, copia los cuatro archivos de E001 y limpia únicamente los datos de la copia; conserva intacto el expediente anterior.
6. Añade el código del proyecto cuando exista un alcance aprobado. Elige su organización según la arquitectura acordada.

La plantilla incluye solo documentación. Antes de publicar tu adaptación, elimina datos sensibles y confirma que todos los campos necesarios estén resueltos. Este repositorio no concede una licencia de distribución: el propietario debe elegirla si desea otorgar permisos de reutilización a terceros.

## Orden de trabajo

Requerimientos → arquitectura → entidades → sistema de diseño → plan de desarrollo → entregas.

Por entrega: **planificar → aprobar alcance → implementar → revisar → corregir → revisar → aprobar entrega**. Si la primera revisión no encuentra pendientes, puede pasar directamente a aprobación humana. Cada transición requiere autorización humana explícita; una aprobación de alcance puede autorizar expresamente las transiciones operativas de implementación, revisión y corrección dentro de ese alcance. Nunca autoriza por sí sola el cierre ni la siguiente entrega.

El silencio, una prueba exitosa o el dictamen favorable de un agente no son aprobación. Un cambio de alcance o de documentos base requiere nueva aprobación antes de implementarse.

## Documentación

Consulta [el índice](docs/README.md), [el flujo y las responsabilidades](docs/agents/WORKFLOW.md) y los prompts de [planificación](docs/agents/PLANNER.md), [desarrollo](docs/agents/DEVELOPER.md) y [revisión](docs/agents/REVIEWER.md).

El expediente E001 es una plantilla pendiente; no representa trabajo ejecutado ni aprobado.
