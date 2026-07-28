### LEN-502 — Verificación Formal y Métodos Formales

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | LEN-201, TEO-303 |
| **ADN institucional** | CMU 15-414 · MIT 6.820 |

**Competencia terminal.** Especifica una propiedad temporal, la verifica mecánicamente y interpreta el contraejemplo cuando falla.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Lógica temporal | Estructuras de Kripke · LTL: sintaxis, semántica, operadores · CTL y CTL* · Expresividad comparada · Especificación de safety y liveness |
| 2 | 4–6 | Model checking | Autómatas de Büchi · Construcción del producto · Model checking explícito · BDDs: construcción, operaciones, reducción, ordenamiento de variables · Model checking simbólico |
| 3 | 7–9 | Model checking acotado y abstracción | Unrolling y codificación SAT · SMT: DPLL(T), teorías de arrays, bitvectors, funciones no interpretadas · CEGAR · Interpretación de contraejemplos |
| 4 | 10–12 | Verificación deductiva | Lógica de Hoare: reglas, consecuencia, bucle con variante e invariante · Correctitud parcial vs total · Weakest precondition (Dijkstra) · Separation Logic: frame rule, bi-abduction |
| 5 | 13–15 | Análisis estático | Interpretación abstracta: retículos, funciones monótonas, conexiones de Galois · Widening y narrowing · Dominios numéricos: intervalos, octágonos, poliedros · Precisión vs escalabilidad |

**Prueba de Dominio.** Verificación formal del algoritmo de exclusión mutua de Peterson en LTL usando SPIN, con interpretación del contraejemplo al debilitar una condición + prueba de correctitud de heapsort con lógica de Hoare e invariantes formalizados y mecanizados en Lean 4 o Rocq.

**Bibliografía.**
- **Base:** *Principles of Model Checking* — Baier & Katoen
- **Complementaria:** *Software Foundations* Vol. 1–3 — Pierce et al. (gratuito) · *The Calculus of Computation* — Bradley & Manna · *Model Checking* (2ª ed.) — Clarke et al.
- **Papers:** *"Separation Logic: A Logic for Shared Mutable Data Structures"* — Reynolds (LICS 2002)

**Recursos.** SPIN/Promela · TLA+ y TLC (Lamport) · Z3 y CVC5 · Lean 4 con mathlib · Rocq (antes Coq) · Dafny · Frama-C.

**Protocolo de estudio.** El asistente de pruebas se usa **después** de tener la prueba en papel, nunca para descubrirla. Buscar la prueba mediante tácticas produce dependencia de la herramienta sin comprensión, y colapsa en cuanto la herramienta no encuentra el camino.

---

