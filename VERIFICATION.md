## 32. Estado de verificación

Los diez puntos que la versión 2026.1 declaraba pendientes. **Verificación realizada el 25/07/2026.** Se declara explícitamente qué se verificó y qué no: tres puntos confirmados, uno confirmado con corrección, seis siguen abiertos.

### 32.1 Verificado — Rocq (antes Coq) ✔ `corregido`

**Confirmado y con cambios operativos que la 2026.1 no recogía.** El asistente de pruebas se renombró oficialmente a **Rocq Prover**; el cambio se anunció en 2024 y se materializó en 2025. Versión estable **9.2.0** (marzo de 2026); la 9.1.1 es de febrero de 2026.

Cambios que afectan a LEN-502, LEN-701 y a §21:

- La biblioteca estándar se dividió en dos: **`Corelib`** (paquete `rocq-core`) y **`Stdlib`** (paquete `rocq-stdlib`, mantenido fuera del repositorio principal).
- El prefijo de importación cambió de `Coq` a `Stdlib`, y es **obligatorio**. Es la causa más común de fallo al seguir material anterior a 2025.
- Un único binario `rocq` despacha compilación, REPL, documentación y cálculo de dependencias.

**Acción aplicada:** nomenclatura actualizada en §21 con nota de compatibilidad. **Acción pendiente para el estudiante:** al llegar a LEN-502, verificar la versión vigente; el ritmo de liberación es de ~2 versiones mayores por año.

**Dato adicional verificado:** Lean estable **4.29.1** (abril de 2026). Relevante para LEN-701 y §22.2.

### 32.2 Verificado — FSRS y configuración de Anki ✔ `confirmado`

La configuración de §12.2 se confirma correcta y se amplía con tres datos que la 2026.1 no tenía:

1. **Rango admitido de retención deseada:** 0.70–0.99 (0.70–0.97 en versiones anteriores a Anki 23.10.1). El valor 0.90 del plan está dentro del rango y es el consenso.
2. **No linealidad del costo:** pasar de 0.90 a 0.95 aproximadamente **duplica** las repeticiones diarias; de 0.95 a 0.97 las vuelve a duplicar. Confirma la elección de 0.90 y explica por qué subirla "para estar más seguro" es una mala operación.
3. **Modo de fallo del algoritmo:** FSRS se adapta a casi cualquier hábito **excepto** pulsar "Hard" en lugar de "Again" cuando se olvidó. Corrompe los datos de entrenamiento del modelo. Incorporado a §12.2 como advertencia.

También confirmado: FSRS es el programador nativo desde Anki 23.10; el optimizador requiere ≥1 000 revisiones (400 en algunas versiones intermedias); existe una función que calcula la retención que minimiza tiempo total de estudio, típicamente entre 0.85 y 0.90.

### 32.3 Verificado — Estándares post-cuánticos del NIST ✔ `ampliado`

La 2026.1 sospechaba que el conjunto podía haberse ampliado. **Se confirma que sí.** Estado a la fecha:

| Estándar | Algoritmo | Origen | Estado |
|---|---|---|---|
| **FIPS 203** | ML-KEM | CRYSTALS-Kyber | Publicado 13/08/2024 |
| **FIPS 204** | ML-DSA | CRYSTALS-Dilithium | Publicado 13/08/2024 |
| **FIPS 205** | SLH-DSA | SPHINCS+ | Publicado 13/08/2024 |
| **FIPS 206** | FN-DSA | FALCON | **En desarrollo** |
| — | HQC | Código, quasi-cíclico | **Seleccionado 11/03/2025** como KEM de respaldo; estándar en desarrollo |

**Consecuencia curricular para SEG-701.** ML-KEM proporciona seguridad IND-CCA2 bajo la dureza de Module-LWE, que conecta directamente con la Prueba de Dominio de la asignatura (demostración IND-CCA2). SLH-DSA es el caso interesante pedagógicamente: su seguridad depende **solo** de propiedades de la función hash, no de dureza de retículos, y es por eso el respaldo si el supuesto de retículos cae. La coexistencia de dos familias con supuestos independientes es un ejemplo de diseño de seguridad que la asignatura debe cubrir explícitamente.

### 32.4 No verificado — Numeración de asignaturas de MIT ✖ `abierto`

Los números **6.890** (complejidad de grano fino, ALG-801) y **6.441[J]** (teoría de la información, TEO-401) **no fueron verificados en esta revisión.** Siguen marcados como dudosos por la renumeración EECS de 2022. Verificar en `eecs.mit.edu` antes de buscar material. El riesgo no es grave: los cursos existen, el número puede haber cambiado.

### 32.5 No verificado — Numeración de CMU, Stanford y UC Berkeley ✖ `abierto`

No verificados. Alto volumen (más de 40 códigos en §19) y bajo riesgo individual. Verificar el código concreto al iniciar cada asignatura, no antes.

### 32.6 No verificado — URL de sitios de curso ✖ `abierto, por diseño`

No se verificaron y **no tiene sentido verificarlos de forma centralizada**: rotan por edición, y varias instituciones archivan ediciones antiguas en subrutas activas. Verificar en el momento de uso. Es la única entrada de esta lista que seguirá abierta permanentemente.

### 32.7 No verificado — Ediciones vigentes de bibliografía ✖ `parcialmente abierto`

Verificadas en la revisión anterior: DDIA 2ª ed. (marzo 2026), CSAPP 3ª ed., CLRS 4ª ed., Strang 6ª ed. (2023). **El resto no se reverificó en esta revisión.** Los borradores en línea (Arora & Barak, Jurafsky & Martin, Prince, Murphy) se actualizan sin cambio de número de edición: descargar la versión del día de inicio de la asignatura, no una copia guardada.

### 32.8 No verificado — Documentación de arquitectura GPU para SIS-702 ✖ `abierto`

Depende de la generación de hardware disponible al estudiante. No verificable en abstracto. La Prueba de Dominio de SIS-702 pide ≥90% del roofline de **la GPU disponible**, no de una GPU de referencia, precisamente por esto.

### 32.9 No verificado — Edición vigente de Stanford CS336 ✖ `abierto`

El contenido de modelado de lenguaje se desactualiza en meses. Verificar `cs336.stanford.edu` al iniciar IAP-801. Es la asignatura del plan con mayor tasa de obsolescencia y la única cuyo material se recomienda no descargar con antelación.

### 32.10 Resuelto — Cotas de carga horaria ✔ `corregido en esta versión`

La 2026.1 declaraba que las cotas de §3.1 eran "estimaciones derivadas de la carga declarada de los cursos fuente, no mediciones". El problema era peor: **no eran estimaciones de nada**, eran cifras inconsistentes con las propias fichas del documento por un factor de 1.7×.

Corregido en §3.2 y §26: las horas ahora se derivan aritméticamente del campo `Carga` de cada ficha y son recalculables. Sigue en pie la advertencia original —las cargas por asignatura son estimaciones de los cursos fuente, no mediciones propias— y sigue siendo obligatorio ajustarlas contra el ritmo real medido tras el primer bloque.

### 32.11 Resumen del estado

| Estado | n | Puntos |
|---|---|---|
| Verificado y confirmado | 2 | FSRS (32.2), NIST PQC (32.3) |
| Verificado con corrección aplicada | 2 | Rocq (32.1), carga horaria (32.10) |
| Abierto — verificar en el momento de uso | 6 | 32.4, 32.5, 32.6, 32.7, 32.8, 32.9 |

**Declaración de alcance.** Esta revisión verificó cuatro de diez puntos. No se afirma haber verificado los otros seis. Un agente o lector que necesite cualquiera de ellos debe verificarlo por su cuenta y anotar la fecha.

---

## 39. Auditoría de integridad de citas — las 39 fichas con ADN institucional

**Auditoría realizada el 29/07/2026.** §32 verificó diez puntos declarados pendientes por la 2026.1. Esta sección hace algo distinto y más amplio: verifica **el campo `ADN institucional` de todas las fichas que lo declaran**, contra la página oficial de la institución citada.

**Era un diagnóstico cuando se escribió.** Ninguna ficha se modificó al redactar esta sección. **La revisión 2026.4 aplicó después las ocho correcciones mecánicas** que aquí se marcan como `corregido en 2026.4`; el resto sigue abierto. Los hallazgos que requieren decisión de contenido están abiertos como issues del repositorio.

### 39.1 Alcance y método

De las 47 unidades del plan, **8 no declaran ADN** —los siete laboratorios integradores y la optativa, todos con `—`. Las **39 restantes** se auditaron íntegramente.

Tres preguntas por ficha: **(1)** ¿existe el curso con ese código en esa institución? **(2)** ¿está vigente, o fue renombrado o descontinuado? **(3)** ¿el temario real cubre lo que la ficha declara, o la cita es inferencia por similitud de título?

| Regla de método | Aplicación |
|---|---|
| Solo fuente primaria | Catálogos oficiales de MIT, Stanford, Berkeley y CMU, y sitios oficiales de curso. **Sin agregadores ni blogs** |
| Doble vía para todo negativo | Ninguna afirmación de inexistencia se emite desde una sola consulta (§39.11) |
| Se declara lo que la página muestra | Si una descripción no menciona un tema, se registra como *no confirmado*, no como *ausente* |

**Resultado agregado.** Los tiers suman 39 y son verificables ficha por ficha:

| Tier | n | Fichas |
|---|---|---|
| **Sin hallazgos** | 5 | SIS-202, TEO-301, LEN-501, SIS-501, SIS-503 |
| **Solo hallazgos menores** | 11 | MAT-101, MAT-102, MAT-302, TEO-302, TEO-303, ALG-401, ALG-402, SIS-701, SEG-701, SEG-702, IAP-603 |
| **Defecto de cita corregible** | 18 | MAT-103, MAT-104, SIS-101, MAT-301, MAT-401, MAT-601, SIS-201, TEO-401, TEO-601, ALG-201, ALG-403, LEN-502, SIS-203, SIS-502, SIS-702, IAP-601, IAP-602, IAP-801 |
| **ADN estructuralmente insuficiente** | 3 | ALG-801, LEN-201, LEN-701 |
| **ADN que no es de asignatura** | 2 | INV-801, INV-802 |

### 39.2 Causa raíz sistémica — la migración a la numeración nueva de MIT quedó a medias ✖ `abierto`

No son ocho errores independientes. Es **un solo evento incompleto**. MIT renumeró EECS en 2022; el plan migró parte de sus citas y dejó el resto en el esquema anterior.

**Los diez números en esquema nuevo existen todos:** `6.1010` `6.1200` `6.1210` `6.1220` `6.1400` `6.1810` `6.1910` `6.3700` `6.5210` `6.5400`.

**Los cinco en esquema antiguo están todos muertos:**

| Número | Fichas | Sucesor identificado |
|---|---|---|
| `6.441` | TEO-401 | 6.7470 / 6.7480, **ambos de posgrado**; la única de pregrado es 18.424, un seminario. **Abierto** — issue #9 |
| `6.820` | LEN-201, LEN-502 | **6.5110** «Foundations of Program Analysis» (posgrado). ✔ **Aplicado en LEN-502 en 2026.4**; en LEN-201 sigue abierto por dominio equivocado (issue #5) |
| `6.826` | LEN-701 | no identificado. **Abierto** — issue #9 |
| `6.829` | SIS-502 | no identificado. **Abierto** — issue #9 |
| `6.890` | ALG-801 | no identificado. **Abierto** — issues #4 y #9 |

**Los dos números `6.Sxxx` fallan igual:** `6.S965` (IAP-801) no existe; `6.S191` (IAP-602) existe solo como contenedor genérico (§39.5). Ambos **abiertos**.

**Dos malformados, de otra naturaleza, ✔ los dos corregidos en 2026.4:** `6.106` era **`6.1060`** (ALG-403, SIS-702) — dígito faltante; y `18.100` exigía variante, ahora **`18.100A/B`** (MAT-103).

**Valor operativo del hallazgo.** Convierte una lista de incidentes en una **regla de barrido mecánica**: todo `6.xxx` de tres dígitos y todo `6.Sxxx` es sospechoso por defecto. La próxima revisión debe auditar por formato de número, no ficha por ficha.

**Limitación declarada.** El catálogo de MIT **no registra números retirados**, de modo que **ninguna de las 12 notas *(ex NNNN)* del plan es verificable por esta vía**. Requieren el crosswalk de renumeración de MIT EECS. La única con corroboración independiente es MAT-104: Tsitsiklis figura como instructor de 6.3700 y es el autor del libro de 6.041.

### 39.3 Apalancamiento — tres correcciones resuelven seis fichas ⚠ `remediación priorizada`

Seis cursos son citados por dos fichas cada uno. En **tres de los seis el curso compartido arrastra el mismo defecto a ambas**, de modo que una corrección resuelve dos síntomas:

| Corrección única | Resuelve | Estado |
|---|---|---|
| `6.820` → **6.5110** | LEN-201, LEN-502 | ✔ **LEN-502 en 2026.4**; LEN-201 abierto (issue #5) |
| `6.106` → **6.1060** | ALG-403, SIS-702 | ✔ **las dos, en 2026.4** |
| Retirar **UC Berkeley CS294** | TEO-601, ALG-801 | ✔ **TEO-601 en 2026.4**; ALG-801 abierto (issue #4) |

**Nota sobre el apalancamiento realizado.** De los tres casos, solo `6.106` se resolvió completo en 2026.4. En los otros dos, la mitad que quedaba fuera lo hacía por una razón asimétrica que solo se ve al intentar aplicarla: **retirar CS294 de ALG-801 la deja sin ninguna fuente**, y **6.5110 es análisis de programas mientras LEN-201 es λ-cálculo**. El apalancamiento existía como oportunidad, pero solo era completo en uno de los tres.

Los otros tres son **repartos legítimos que el plan no declara** y que deberían figurar como tales en vez de como fuente independiente en cada ficha:

| Curso | Reparto real |
|---|---|
| MIT 6.5400 (=18.404[J]) | TEO-301 toma computabilidad; TEO-302, complejidad |
| CMU 15-210 | ALG-201 toma la mitad secuencial; ALG-403, la paralela |
| CMU 15-445 | SIS-503 lo sostiene entero; la reclamación de SIS-203 es débil (§39.4) |

### 39.4 Patrón A — la segunda fuente que no sostiene nada ✖ `abierto`

Una fuente fuerte y bien elegida, más una segunda que tiene la firma de haberse elegido por afinidad de título y no por lectura de sílabo.

| Ficha | Sostiene | No sostiene |
|---|---|---|
| SIS-101 | CMU 15-122 | **MIT 6.1010 es un curso de Python.** Descripción oficial: *«programming and Python basics… data types, and recursion»*. La ficha declara C, `malloc/free`, `valgrind`, GDB y desensamblado |
| MAT-401 | Stanford EE364A/B | **MIT 18.085 no cubre ninguna de las cinco unidades.** Es «Computational Science and Engineering I»: elementos finitos, Laplace, Fourier, MATLAB. Sin optimización convexa, dualidad, KKT ni punto interior |
| MAT-601 | MIT 18.950 (parcial) | **Stanford CS468 es *geometric computing***, no geometría diferencial: shape matching, planificación de movimiento, detección de colisiones |
| SIS-502 | Stanford CS144 | MIT 6.829 — no existe |
| IAP-801 | Stanford CS336 | MIT 6.S965 — no existe |
| SIS-702 | CMU 15-418/618 | `6.106` mal escrito **y** CS315A dormido desde 2018 |

**Dos casos adicionales de desajuste de dominio,** de la misma familia pero con una sola fuente:

- **SIS-203 cita un curso de bases de datos y sus dos primeras unidades son de sistemas operativos.** U1 es memoria virtual, TLB y tablas PML4; U2 son políticas de reemplazo. **CMU 15-445 no cubre memoria virtual en ninguna parte.** Solo la U5 (buffer pool, pinning, latching) es contenido genuino suyo.
- **LEN-502 cita CMU 15-414, cuyo título real es «Bug Catching: Automated Program Verification and Testing» y cuya herramienta es Why3.** No confirma LTL/CTL, autómatas de Büchi, BDDs, model checking acotado ni interpretación abstracta — las unidades 1, 2, 3 y 5 de la ficha. Y la Prueba de Dominio exige **SPIN**, que no aparece.
- **LEN-201 cita CMU 15-150, que es un curso de programación en ML.** Sus objetivos son escribir programas ML bien tipados, recursión con inducción y diseño de módulos. **No menciona λ-cálculo, sistemas de tipos como teoría, inferencia de tipos ni Curry-Howard**, que son las cinco unidades de la ficha.

### 39.5 Patrón B — ADN de contenido variable ✖ `abierto`

Cinco cursos citados como ADN **declaran que su contenido cambia por oferta**. Los cinco comparten la marca formal de que la institución no fija su alcance: **son repetibles para crédito**.

| Curso | Fichas | Evidencia textual de la fuente primaria |
|---|---|---|
| **MIT 18.217** | MAT-301 | «Combinatorial Theory», nivel G, prereq *permission of instructor*. *«Content varies from year to year»*, *«Can be repeated for credit»* |
| **Stanford CS468** | MAT-601 | *«Advanced seminar covering different topics related to geometric computing»*, repetible. Última oferta listada en la página oficial: **2013** |
| **UC Berkeley CS294** | TEO-601, ALG-801 | **«CS 294. Special Topics»**, *«Topics will vary from semester to semester»*. **No es un curso**: es un número con múltiples secciones simultáneas, cada una con sílabo y prerrequisitos propios |
| **CMU 15-819** | LEN-701 | «Homotopy Type Theory», Harper, **Fall 2013**. Seminario de investigación de posgrado; el número designa materia variable |
| **MIT 6.S191** | IAP-602 | **«Special Laboratory Subject in EECS»** · IAP · **«Units arranged [P/D/F]»** · repetible · permiso del instructor |

**Por qué es un error de categoría y no de cita.** §1 establece que el ADN fija *«el alcance, la profundidad demostrativa y el proyecto terminal»*. Un curso que no fija su propio alcance no puede fijar el de otro. El plan trata todos sus cursos fuente como si tuvieran temario estable, y cinco no lo tienen.

**6.S191 es el caso más severo, y su problema es de calibración.** Es un slot de laboratorio del término de enero (IAP, cuatro semanas), **sin nota numérica** y **sin carga declarada**. IAP-602 son 5 créditos, 18 h/semana, 16 semanas y dificultad 9/10. Replicar fielmente la fuente **degradaría** la asignatura en lugar de sostenerla.

### 39.6 Patrón C — ADN de posgrado para ficha de pregrado ⚠ `declarar, no corregir`

Nueve fichas de pregrado citan cursos de posgrado. Varios son cursos que estudiantes avanzados de pregrado cursan con normalidad, así que **no es necesariamente un defecto** — pero no está declarado, y en dos casos tiene consecuencias:

`18.217` (MAT-301, con *permission of instructor*) · `8.370[J]/18.435[J]` (TEO-601) · `6.5210[J]` (ALG-402, **15 unidades, primer año de posgrado**) · `6.5110` (LEN-201, LEN-502, si se aplica la corrección) · `6.5840` (SIS-701) · `6.5620[J]` (SEG-701) · `15-819` (LEN-701) · `6.7470`/`6.7480` (sucesores de 6.441, TEO-401).

**Consecuencia dura, en TEO-601:** ver §39.8.

### 39.7 Patrón D — Prueba de Dominio sin anclaje en ninguna fuente citada ✖ `abierto`

Categoría distinta de la sobreafirmación de unidad: aquí **el artefacto que decide la aprobación de la asignatura** no está respaldado por nada de lo que la ficha declara como su ADN.

| Ficha | Instrumento que decide la aprobación | Estado |
|---|---|---|
| **ALG-201** | Análisis amortizado de Fibonacci heaps por función potencial | Ni 6.1210 ni 15-210 los cubren |
| **LEN-701** | Formalización en Lean 4 / Rocq con extracción certificada | **Ninguna de las tres fuentes cubre asistentes de prueba**; 15-317 lo niega explícitamente |
| **IAP-601** | Cota PAC vía dimensión VC + dual del SVM + convergencia de EM | **2 de 3 componentes sin fuente**: ni CS229 ni CS189 cubren PAC ni VC |

**Sub-patrón de remediación barata: la fuente correcta ya está en el plan, citada por otra ficha.** Cinco huecos se cierran moviendo o añadiendo una cita que el propio plan ya contiene:

| Hueco | Fuente ya presente en el plan | Estado |
|---|---|---|
| ALG-201 · heaps y análisis amortizado | **6.1220** los lista — es el ADN de ALG-401 | Abierto: cierre parcial (issue #6) |
| IAP-602 U5 · mixture-of-experts | **CS336** lo cubre — es el ADN de IAP-801 | Abierto: cierre parcial |
| LEN-502 · model checking e interpretación abstracta | **6.5110** los cubre — es el sucesor de su propia cita muerta | ✔ **aplicado en 2026.4** |
| SIS-201 U3 · procesador segmentado | **6.1910** lo lista — es el ADN de SIS-202 | Abierto: cierre parcial |
| SIS-203 U1–U2 · memoria virtual y TLB | **6.1810** los cubre — es el ADN de SIS-501 | ✔ **aplicado en 2026.4** |

Tres de los cinco son cierres **parciales** y por eso siguen abiertos: 6.1220 lista *heaps* y análisis amortizado pero no nombra Fibonacci heaps; 6.1910 lista procesador segmentado pero no predicción de saltos ni ejecución especulativa; CS336 cubre MoE pero no S4/Mamba ni atención lineal. **Los dos que se aplicaron en 2026.4 eran cierres completos.**

### 39.8 Hallazgos estructurales de ficha única ✖ `abierto`

**ALG-801 — la única ficha sin ningún ADN verificable.** MIT 6.890 no existe (sin resultado por número ni por tema) y UC Berkeley CS294 no es un curso. La atribución «(R. Williams & V. Vassilevska Williams)» tampoco es verificable. Es dificultad 10/10 del Ciclo VIII, con Prueba de Dominio sobre la cota SETH para Edit Distance y construcción de un PCP.

**LEN-701 — tres fuentes, tres modos de fallo distintos.** 15-317 existe y cubre 1 de 5 unidades; 15-819 es un seminario de temas cuya oferta citada es de 2013; 6.826 no existe. Más el Patrón D sobre su Prueba de Dominio.

**TEO-601 — brecha de prerrequisito, y la cita es correcta.** 8.370[J]/18.435[J] existe, el emparejamiento de números es exacto y sus instructores son Chuang, Harrow y Shor. El problema es que **exige 8.05 (Quantum Physics II)** y **el plan no contiene mecánica cuántica en ninguna de sus 47 unidades**; los prerrequisitos que asigna son MAT-102, MAT-302 y TEO-302. El plan declara derivar exigencia de un curso para el que no prepara. Se corrige acotando el alcance de la ficha o declarando la brecha, **no cambiando la cita**.

### 39.9 ADN de programa o mecanismo institucional, no de asignatura ⚠ `categoría nueva`

INV-801 e INV-802 no citan códigos de curso, citan tipos de programa. No son verificables contra catálogo, y **los dos casos difieren en algo esencial**:

**INV-802 — cita falsificable, y falsificada.** Su ADN es «MIT UROP · CMU Senior Thesis · Stanford Honors Program». Son programas reales e identificables, así que la cita **sí admite verificación**. UROP, contra su sitio oficial, es un **sistema de emparejamiento y apoyo a la investigación, no un curso**: el estudiante busca proyectos en una base de datos y postula; las modalidades incluyen **financiamiento directo, crédito o voluntariado**; **no tiene currículo fijo, no exige tesis ni paper, y no tiene evaluación estándar** —depende del mentor. INV-802 es una tesis de 40–80 páginas con contribución original y defensa ante ≥3 doctores, 8 créditos y 26 h/semana. **UROP no puede establecer alcance, profundidad ni proyecto terminal porque no tiene ninguno de los tres.** Las otras dos citas no se pudieron verificar y son, estructuralmente, sí tesis.

**INV-801 — cita inherentemente no falsificable, y hay que decirlo así.** Su ADN es *«Seminario doctoral de MIT, CMU, Stanford y Berkeley, adaptado a pregrado»*. **No nombra ningún objeto.** No existe tal entidad: cada departamento de cada institución dicta múltiples seminarios doctorales con números y formatos distintos. No hay nada que buscar en un catálogo ni nada que pueda resultar falso. Es la única de las 39 en esa condición. Un campo cuyo propósito declarado es hacer auditable el nivel de exigencia, redactado de modo que no admite auditoría, no cumple su función — con independencia de que la descripción sea razonable en espíritu.

### 39.10 Vigencia y otros hallazgos transversales ⚠ `verificar en el momento de uso`

**Seis páginas de curso posiblemente estancadas:** Stanford CS468 (2013) · CMU 15-819 (2013) · CMU 15-317 (2017) · **Stanford CS315A (2018, solo un directorio `restricted/`)** · Stanford EE376A (2018-19) · Stanford CS261 (2023-24).

**Dos avisos de vigencia activa:** **6.5210[J]** (ALG-402) *no se dicta en 2025-2026*, programada para otoño de 2026-27. Y la edición **«Spring 2026» de CS336** (IAP-801) sigue sin confirmar: la página que responde es el archivo de Spring 2025 y declara que existe una oferta posterior, sin identificarla. **Esto mantiene §32.9 abierto tal como el plan ya lo declaraba.**

**Una cita fuera del marco institucional de §1:** **Harvard Stat 110** en MAT-104. §1 declara que el ADN proviene de MIT, CMU, Stanford o UC Berkeley; Harvard no está en ese conjunto, exista el curso o no.

**Dos correcciones de detalle en SIS-201:** la referencia cruzada `18-213` no aparece en la fuente primaria, que se titula «15-213/15-503»; y la lista de laboratorios de la ficha declara un «L5 performance lab» que **no existe** entre los nueve labs vigentes (`cprogramminglab, datalab, bomblab, attacklab, cachelab, malloclab, tshlab, proxylab, sfslab`).

**Los mejores ADN del plan**, registrados porque demuestran que los patrones anteriores son evitables y no inherentes al diseño:

| Ficha | Por qué |
|---|---|
| **TEO-301** | 18.404[J]/6.5400[J] verificado con **Sipser como instructor**; cubre las cinco unidades |
| **LEN-501** | CS143 (frontend) + 15-411 (backend). **Reparto por capas**: SSA falta en la primera y está confirmada en la segunda |
| **SIS-503** | 15-445/645 con **Pavlo** verificado; sostiene las cinco unidades |
| **SEG-701** | 6.5620[J]/18.425[J] con Goldwasser, Micali y Vaikuntanathan; emparejamiento exacto |
| **SIS-502** | CS144, cuyos checkpoints 2–6 **son** la Prueba de Dominio de la ficha, punto por punto |

### 39.11 Limitaciones declaradas de esta auditoría ✖ `abierto por método`

**Un falso negativo detectado y corregido, y la regla que impuso.** En el primer lote, la página de listado de Course 6 del catálogo de MIT reportó **6.3700 como inexistente**. Era truncamiento al convertir la página a texto: la búsqueda dirigida devolvió el curso completo, con título, unidades e instructores. Desde entonces **todo negativo se confirmó por segunda vía**. Sin ese control, esta auditoría habría declarado muerto un curso vivo.

Consecuencia metodológica que queda como regla: de una página de listado, **los positivos son fiables y los negativos no valen nada**. La verificación por número individual sí es fiable en ambos sentidos.

**Nueve fuentes no verificadas.** Es una limitación del método, **no un hallazgo negativo sobre el plan**, y no debe leerse como tal:

| Fuente | Ficha | Motivo |
|---|---|---|
| UC Berkeley MATH 113 | MAT-302 | Rutas de catálogo de Berkeley: redirección al registrador y 404 |
| UC Berkeley Math 125A | TEO-303 | Ídem |
| CMU 21-701 | MAT-301 | `ECONNREFUSED` en el catálogo, 404 en el departamento |
| CMU 15-312 | LEN-201 | 404 en el sitio oficial. **Pesa**: es la fuente que sostendría la teoría de la ficha |
| CMU 15-330 | SEG-702 | 404 en dos rutas |
| Stanford CS145 | SIS-203 | La URL oficial devuelve un listado de directorio |
| Contenido de UC Berkeley CS188 | IAP-603 | Existencia y título sí; temario no |
| CMU Senior Thesis | INV-802 | 404 |
| Stanford Honors Program | INV-802 | No consultado |

**Lo que esta auditoría no hizo.** No verificó las notas *(ex NNNN)* (§39.2), ni la bibliografía de las fichas, ni los recursos, ni si los cursos citados aceptan estudiantes externos. Verificó el campo ADN y su correspondencia con las unidades declaradas, nada más.

**Omisión de la auditoría, detectada al aplicar 2026.4.** Esta sección auditó el campo ADN de las fichas y **no advirtió que está duplicado**: la misma cita vive en la ficha, en la fila correspondiente de la malla curricular del `README.md`, y a veces una tercera vez en el campo `Recursos` de la propia ficha. Las recomendaciones de remediación de §39.3 y §39.7 decían «corregir el campo ADN» sin señalar que hay dos o tres copias, y la revisión 2026.4 lo descubrió al dejar momentáneamente seis fichas contradiciendo a su índice. La regla correctiva quedó como checklist permanente en `CONTRIBUTING.md` y registrada en §38.5 de `CHANGELOG.md`.

### 39.12 Resumen del estado

| Categoría | n |
|---|---|
| Fichas auditadas | **39 de 39** |
| Fuentes primarias confirmadas | 46 |
| Números MIT inexistentes | 6 (`6.441`, `6.820`, `6.826`, `6.829`, `6.890`, `6.S965`) |
| Números malformados | 2 (`6.106`→`6.1060`, `18.100` sin variante) |
| **Patrón A** — segunda fuente que no sostiene | 6 fichas + 3 de desajuste de dominio |
| **Patrón B** — ADN de contenido variable | 5 cursos / 6 fichas |
| **Patrón C** — ADN de posgrado para pregrado | 9 fichas |
| **Patrón D** — Prueba de Dominio sin anclaje | 3 fichas |
| Correcciones de apalancamiento disponibles | 3 (resuelven 6 fichas) |
| Huecos cerrables con una cita ya presente en el plan | 5 (3 de ellos parciales) |
| Fichas sin ADN verificable | 1 (ALG-801) |
| ADN estructuralmente insuficiente | 3 (ALG-801, LEN-201, LEN-701) |
| ADN no falsificable por diseño | 1 (INV-801) |
| Brechas de prerrequisito | 1 (TEO-601 ← 8.05) |
| Páginas posiblemente estancadas | 6 |
| Fuentes no verificadas por límite de método | 9 |

**Declaración de alcance.** Esta auditoría verificó las 39 fichas con ADN declarado. **No se afirma haber verificado las nueve fuentes de §39.11**, ni ninguna nota *(ex NNNN)*. Un lector o agente que necesite cualquiera de ellas debe verificarla por su cuenta y anotar la fecha.

**Estado tras la revisión 2026.4.** Se aplicaron **ocho de los hallazgos**, todos mecánicos y verificados, sobre seis fichas: MAT-103, SIS-203, ALG-403, LEN-502, TEO-601 y SIS-702. El registro está en §38 de `CHANGELOG.md`. Los defectos restantes de §39.2 siguen abiertos por falta del crosswalk de renumeración, y los cinco casos estructurales de §39.7–§39.9 siguen esperando decisión, cada uno en su issue.

**Condición de cierre.** §39 se cierra cuando los defectos restantes de §39.2 estén corregidos y los cinco casos estructurales tengan decisión declarada. Hasta entonces queda abierta, y **el campo ADN del plan debe leerse como indicativo y no como verificado**, salvo en las cinco fichas de §39.10 y en las seis corregidas en 2026.4.

---

