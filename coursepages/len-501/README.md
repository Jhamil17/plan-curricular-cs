### LEN-501 — Diseño de Compiladores — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | LEN-201, TEO-301, SIS-201 |
| **ADN institucional** | Stanford CS143 · CMU 15-411 |

**Competencia terminal.** Construye un compilador completo con optimizaciones que preservan la semántica demostrablemente.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Análisis léxico y sintáctico | Regex → NFA (Thompson) → DFA (construcción de subconjuntos) · Gramáticas LL(1) · LR(0), SLR(1), LALR(1), LR(1) · Construcción de tablas · Recuperación de errores |
| 2 | 4–6 | Análisis semántico | AST · Tabla de símbolos y ámbitos · Sistemas de tipos · Chequeo e inferencia (algoritmo W de LEN-201) · Errores semánticos |
| 3 | 7–9 | Representación intermedia | IR de tres direcciones · SSA · Dominadores y fronteras de dominancia · Inserción de funciones φ · Salida de SSA |
| 4 | 10–12 | Análisis y optimización | Dataflow: reaching definitions, live variables, available expressions · Retículo y punto fijo · Eliminación de código muerto · Propagación de constantes y de copias · LICM · Análisis de variables de inducción · Desenrollado · Análisis de alias: Andersen vs Steensgaard |
| 5 | 13–15 | Generación de código | Selección de instrucciones · Asignación de registros por coloración de grafos de interferencia · Spilling · Convenciones de llamada x86-64 · Planificación de instrucciones · Peephole · SIMD |

**Prueba de Dominio.** Compilador completo y funcional desde un lenguaje tipo C simplificado hasta x86-64, con: análisis léxico, parsing LALR(1), inferencia de tipos, representación SSA, al menos cuatro optimizaciones dataflow y asignación de registros por coloración. Cada optimización acompañada de un test de regresión que falla si la optimización rompe la semántica.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del compilador y se declara su escalamiento respecto al tamaño del programa de entrada —por fase, con el paso dominante identificado—, contrastado contra la complejidad derivada.

**Bibliografía.**
- **Base:** *Engineering a Compiler* (3ª ed., 2022) — Cooper & Torczon
- **Complementaria:** *Modern Compiler Implementation in ML* — Appel · *Compilers: Principles, Techniques, and Tools* — Aho, Lam, Sethi & Ullman (el "dragon book") · *SSA-based Compiler Design* — Rastello & Bouchez (gratuito)
- **Papers:** *"Efficiently Computing Static Single Assignment Form and the Control Dependence Graph"* — Cytron et al. (TOPLAS 1991)

**Recursos.** web.stanford.edu/class/cs143 · CMU 15-411 · LLVM (documentación de IR y de pases) · Compiler Explorer · Alive2 para verificar que una optimización preserva semántica.

**Protocolo de estudio.** La suite de regresión se escribe **antes** que la optimización. Toda optimización aceptada sin test que la contradiga es una fuente de bugs que aparecerán a diez pases de distancia.

---

