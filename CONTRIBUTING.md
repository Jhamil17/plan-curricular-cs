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

El archivo de §37 corrige los tres: número fijo, contador de subsecciones independiente del de los registros, y domicilio conocido de antemano. Los registros de cambios siguen tomando **el siguiente entero de nivel superior que esté libre**; el archivo no se mueve.

**No se enumeran números futuros.** La primera redacción de esta convención decía «(§38, §39, …)», y quedó inexacta en cuanto §39 se asignó a la auditoría de citas de `VERIFICATION.md`. Un número solo se declara reservado cuando se reserva: **§38 está reservada para el registro 2026.3 → 2026.4**; los siguientes se asignan al usarse, consultando primero qué está ocupado.

**Obligación al migrar.** Corregir toda referencia que apunte a la nota en su ubicación anterior —enlaces, anchors y menciones en prosa desde cualquier archivo del repositorio— en el mismo commit que la mueve. Una nota migrada que deja referencias colgando es peor que una nota acumulada.

## Checklist para editar el campo `ADN institucional`

**El campo está duplicado, y a veces triplicado.** No es un campo único por asignatura: la misma cita vive en varios lugares que hay que mantener sincronizados a mano. Corregir solo uno deja el plan contradiciéndose a sí mismo.

Antes de dar por cerrada cualquier edición de ADN, recorrer los cinco puntos:

- [ ] **1. La ficha.** `coursepages/<código>/README.md`, fila `**ADN institucional**` de la tabla de cabecera.
- [ ] **2. La malla curricular del `README.md`.** La fila de esa asignatura en la tabla de su ciclo, última columna. **Es la que se olvida.**
- [ ] **3. El campo `Recursos` de la ficha.** Algunas fichas repiten ahí el número del curso fuente. No todas: hay que mirar.
- [ ] **4. Verificar contra catálogo oficial antes de publicar**, no después. Fuente primaria: catálogo de la institución o sitio oficial del curso. Nunca agregadores.
- [ ] **5. Cerrar con `grep`.** La edición no está completa hasta que buscar el código viejo en todo el repositorio devuelve solo menciones históricas:

```
grep -rn "<código viejo>" . --include=*.md
```

**Las menciones históricas se conservan.** `CHANGELOG.md` y `VERIFICATION.md` deben seguir citando el número viejo: son el registro de qué se corrigió y cuándo, y borrarlo destruiría la trazabilidad. Todo lo demás debe estar limpio.

**Regla de sospecha por formato.** Antes de confiar en cualquier número de MIT ya presente en el plan: **todo `6.xxx` de tres dígitos y todo `6.Sxxx` es sospechoso por defecto.** MIT renumeró EECS en 2022 y el plan quedó a medio migrar; §39.2 de `VERIFICATION.md` documenta que los cinco números en esquema antiguo que citaba estaban todos muertos, y los diez en esquema nuevo, todos vivos. Un barrido por formato de número encuentra la clase entera de error más rápido que auditar ficha por ficha.

**Procedencia de este checklist.** No es preventivo en abstracto: la revisión 2026.4 corrigió las fichas y olvidó la malla del `README.md`, dejando durante dos commits seis fichas que contradecían a su propio índice. La auditoría de §39, que había recomendado las correcciones, tampoco advirtió la duplicación. Ver §38.5 de `CHANGELOG.md`.
