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

