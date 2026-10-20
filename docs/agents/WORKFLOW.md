# Flujo de trabajo

## Responsabilidades

| Rol | Responsabilidad | Límite |
| --- | --- | --- |
| Persona responsable | Define prioridades, resuelve dudas y autoriza avances y cierres | Solo ella aprueba |
| Planificador | Prepara documentos base, plan y alcance verificable | No implementa ni aprueba |
| Desarrollador | Implementa y corrige dentro del alcance autorizado; aporta evidencia | No amplía alcance ni se aprueba |
| Revisor | Contrasta código y evidencia con lo aprobado; registra hallazgos y verifica correcciones | No corrige código ni concede aprobación humana |

Asigna una sesión separada para el revisor y dale acceso al mismo estado del trabajo. Si no puede comprobar algo, lo declara pendiente. Cada agente lee su prompt y este flujo al iniciar.

## Preparación

Completar y obtener aprobación humana de requerimientos → arquitectura → entidades → sistema de diseño → plan. Registrar cada aprobación en el documento correspondiente. Una propuesta técnica no se convierte en decisión por estar escrita. Las dudas bloqueantes se resuelven con la persona responsable.

## Secuencia de cada entrega

1. **Planificar:** el planificador crea SCOPE.md a partir de las bases aprobadas y define criterios y verificaciones.
2. **Aprobar alcance:** la persona registra en APPROVAL.md el alcance y las versiones exactas aprobadas, y las acciones autorizadas. Sin ese registro no se implementa.
3. **Implementar:** el desarrollador ejecuta lo autorizado y añade una entrada en IMPLEMENTATION.md con cambios, referencia del trabajo y evidencia.
4. **Revisar:** con autorización humana, el revisor verifica ese estado y añade R01 a REVIEW.md. Un dictamen favorable solo recomienda el cierre.
5. **Corregir:** la persona autoriza las correcciones; el desarrollador añade C01 en IMPLEMENTATION.md y relaciona cada cambio con un hallazgo. No altera la revisión anterior.
6. **Revisar de nuevo:** con autorización humana, el revisor añade R02, verifica correcciones y regresiones y marca cada hallazgo resuelto, abierto o no verificable con evidencia. Repetir C02/R03 según sea necesario.
7. **Aprobar entrega:** con criterios satisfechos y sin hallazgos pendientes, la persona aprueba el estado exacto revisado en APPROVAL.md. Debe autorizar expresamente el inicio de la siguiente entrega.

La autorización humana de alcance puede cubrir expresamente implementar, revisar y repetir correcciones/revisiones dentro del alcance. Si no lo hace, solicitar autorización en cada transición. Registrar sus términos en APPROVAL.md. Nunca inferir permiso por silencio, por el tiempo transcurrido o por recomendaciones de agentes.

## Cambios e historial

- Usar E001, E002, etc. Cada expediente contiene solo SCOPE.md, IMPLEMENTATION.md, REVIEW.md y APPROVAL.md.
- Añadir entradas fechadas con identificador en los mismos archivos. No crear archivos por ronda ni sobrescribir evidencia, decisiones o revisiones anteriores.
- SCOPE.md conserva sus versiones completas en secciones sucesivas si cambia; señalar cuál está vigente.
- Si cambia el alcance o una base aprobada, detener trabajo afectado, describir impacto, actualizar versiones y obtener aprobación humana antes de seguir. Conservar el historial y revisar de nuevo los cambios afectados.
- Una aprobación corresponde al estado citado. Cambiar el trabajo tras la última revisión exige nueva revisión y aprobación antes del cierre.
- Registrar rechazos, solicitudes de cambios y autorizaciones revocadas; una decisión nueva sustituye explícitamente a la anterior, sin borrarla.

## Evidencia y cierre

Cada criterio del alcance debe vincularse con una comprobación real: método o comando exacto, fecha, entorno, versión del trabajo, resultado esperado, resultado observado y salida relevante o enlace estable a la evidencia. Para interfaz, incluir comprobación visual y estados relevantes. Se permiten evidencias insertadas o enlazadas en estos archivos sin crear carpetas adicionales.

No inventar pruebas, capturas, resultados, firmas ni aprobaciones. Distinguir «No ejecutado», «Falló» y «Pasó». Si faltan accesos o entorno, documentar el bloqueo; una prueba prevista no cuenta como ejecutada. No incluir secretos ni datos personales innecesarios.

Cierre: todos los criterios comprobados, hallazgos resueltos y verificados, documentación consistente, revisión favorable sobre el estado vigente y aprobación humana explícita. Un criterio incumplido requiere corregir o modificar y aprobar el alcance; no se omite silenciosamente.
