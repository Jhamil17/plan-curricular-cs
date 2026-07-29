# Contribuir

Este es un currículo personal de autoestudio, no un proyecto comunitario como OSSU. Aun así, si encuentras:

- un curso fuente caído o reemplazado,
- un error aritmético en créditos/horas,
- una inconsistencia entre fichas y las tablas de resumen,

abre un Issue o edita directamente y documenta el cambio en `CHANGELOG.md`, siguiendo el formato usado en el registro 2026.1 → 2026.2 (defecto encontrado → corrección aplicada → sección afectada).

## Proceso de versionado

Cada revisión mayor (2026.1, 2026.2, ...) debe:

1. Declarar qué defecto motivó la revisión.
2. Listar secciones nuevas, ampliadas y sin cambios.
3. Conservar intactas las fichas de asignaturas salvo que el defecto esté en la ficha misma.

## Convención de notas de revisión

El `README.md` conserva **únicamente la nota de la revisión vigente**. Al publicarse una revisión nueva, la nota de la anterior **migra a `CHANGELOG.md`**, como subsección `§NN.0` del registro de cambios que le corresponde, con una advertencia de que sus referencias a "esta versión" son a la versión que documenta.

**Por qué.** Una nota de revisión existe para condicionar la lectura del documento vigente; acumularlas en el README convierte la portada en un historial y obliga al lector nuevo a distinguir qué advertencia sigue en vigor. El historial es función del `CHANGELOG.md`.

**Obligación al migrar.** Corregir toda referencia que apunte a la nota en su ubicación anterior —enlaces, anchors y menciones en prosa desde cualquier archivo del repositorio— en el mismo commit que la mueve. Una nota migrada que deja referencias colgando es peor que una nota acumulada.
