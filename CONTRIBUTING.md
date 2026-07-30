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

El `README.md` conserva **únicamente la nota de la revisión vigente**. Al publicarse una revisión nueva, la nota de la anterior **migra al archivo de notas de revisión de `CHANGELOG.md` (§37)**, como la siguiente subsección libre de ese archivo, en orden de migración.

**Formato de la subsección migrada.** Encabezado con la revisión y la ventana de calendario durante la cual fue vigente, más una advertencia de que sus referencias a "esta versión" apuntan a la versión que documenta:

```
### 37.N Nota de la revisión AAAA.M · vigente del DD/MM/AAAA al DD/MM/AAAA
```

**Por qué un archivo y no una subsección de cada registro.** Una nota de revisión existe para condicionar la lectura del documento vigente; acumularlas en el README convierte la portada en un historial y obliga al lector nuevo a distinguir qué advertencia sigue en vigor. Pero repartirlas como subsección de cada registro de cambios tiene tres defectos propios, y por eso se descartó:

1. **`§NN.0` no existe en la numeración de este documento.** Toda subsección empieza en `.1`; un índice cero es un hueco inventado para colar la nota antes de `§NN.1`.
2. **No produce un archivo, produce N huérfanas.** Con cinco revisiones las notas viven en cinco secciones distintas, y un lector que pregunte "qué advirtió cada revisión" tiene que saltar entre ellas.
3. **Acopla la nota al número del registro.** La nota de la revisión vigente no tendría domicilio asignado hasta que la revisión *siguiente* creara su registro, de modo que la convención no puede decir dónde vivirá una nota antes de que deje de estar vigente.

El archivo de §37 corrige los tres: número fijo, contador de subsecciones independiente del de los registros, y domicilio conocido de antemano. Los registros de cambios siguen tomando el siguiente entero de nivel superior (§38, §39, …); el archivo no se mueve.

**Obligación al migrar.** Corregir toda referencia que apunte a la nota en su ubicación anterior —enlaces, anchors y menciones en prosa desde cualquier archivo del repositorio— en el mismo commit que la mueve. Una nota migrada que deja referencias colgando es peor que una nota acumulada.
