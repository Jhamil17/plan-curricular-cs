### LEN-201 — Lenguajes de Programación y Semántica — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 10 · **16 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-101, SIS-101 |
| **ADN institucional** | CMU 15-150, 15-312 · MIT 6.820 |

**Competencia terminal.** Define la semántica de un lenguaje mediante reglas de inferencia y demuestra propiedades de su sistema de tipos.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | λ-cálculo | λ-cálculo sin tipo · Reducción β y η · Confluencia (Church-Rosser) · Normalización · Codificaciones de Church · Punto fijo (Y) |
| 2 | 4–6 | Sistemas de tipos | λ-cálculo tipado simple · Seguridad de tipos: progreso y preservación · Tipos algebraicos (ADTs) · Polimorfismo paramétrico vs ad-hoc · Sistema F |
| 3 | 7–9 | Inferencia de tipos | Hindley-Milner · Unificación · Algoritmo W · Demostración de corrección y completitud · Let-polimorfismo |
| 4 | 10–12 | Semántica formal | Operacional small-step (SOS) y big-step · Denotacional: dominios de Scott, punto fijo de Tarski · Axiomática: lógica de Hoare, correctitud parcial vs total |
| 5 | 13–15 | Efectos y control | Sistemas de efectos · Mónadas · Continuaciones y transformación CPS · Correspondencia de Curry-Howard |

**Prueba de Dominio.** Demostración formal de la correctitud del algoritmo W por inducción estructural sobre derivaciones de tipo + intérprete de λ-cálculo tipado con polimorfismo paramétrico, con verificación experimental de progreso y preservación sobre un banco de programas.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del intérprete, con el escalamiento declarado respecto al tamaño del término. El número que decide algo es el **costo comparado de las estrategias de reducción**: sobre el mismo banco de programas, orden normal y orden aplicativo difieren en número de reducciones —y en si terminan—, de modo que la medición es lo que justifica la estrategia implementada en vez de heredarla del libro. Conecta con Church-Rosser: la confluencia garantiza el mismo resultado, no el mismo costo.

**Bibliografía.**
- **Base:** *Types and Programming Languages* — Pierce (TAPL)
- **Complementaria:** *Practical Foundations for Programming Languages* (2ª ed.) — Harper · *The Formal Semantics of Programming Languages* — Winskel
- **Papers:** *"A Theory of Type Polymorphism in Programming"* — Milner (1978)

**Recursos.** CMU 15-312 notas públicas · *Software Foundations* Vol. 1 (Pierce et al., gratuito) · OCaml o Standard ML como lenguaje de implementación · Redex/PLT para prototipar semánticas.

**Protocolo de estudio.** Las reglas de inferencia se reproducen de memoria en notación de secuentes. Tarjeta estándar de la asignatura: dado un juicio de tipado, reconstruir el árbol de derivación completo.

---

