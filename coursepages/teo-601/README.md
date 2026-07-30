### TEO-601 — Computación Cuántica: Teoría y Algoritmos

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-102, MAT-302, TEO-302 |
| **ADN institucional** | MIT 8.370[J] / 18.435[J] · UC Berkeley CS294 |

**Competencia terminal.** Deriva algoritmos cuánticos desde primeros principios y sitúa BQP respecto de las clases clásicas.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Formalismo | Espacios de Hilbert · Notación de Dirac: bras, kets, operadores · Producto tensorial · Qubit y esfera de Bloch · Medición y colapso · Entrelazamiento y desigualdad de Bell |
| 2 | 4–6 | Circuitos | Unitariedad y reversibilidad · Hadamard, Pauli, CNOT, Toffoli, T · Universalidad de conjuntos de compuertas · Rotaciones en SU(2) · Teorema de Solovay-Kitaev · No-cloning |
| 3 | 7–9 | Algoritmos fundamentales | Deutsch-Jozsa · Bernstein-Vazirani · Simon · Quantum Fourier Transform con construcción O(n²) · Estimación de fase |
| 4 | 10–12 | Shor y Grover | Reducción de factorización a order-finding · Shor completo con análisis de probabilidad de éxito · Grover: O(√N), interpretación geométrica, optimalidad de la cota · Amplitude amplification |
| 5 | 13–15 | Errores y complejidad | Código de Shor · Formalismo de estabilizadores · Toric code · Umbral de tolerancia a fallos · BQP y QMA · Relación con P, NP, PSPACE · Muestreo de circuitos aleatorios |

**Prueba de Dominio.** Derivación completa del algoritmo de Shor desde la reducción de factorización a order-finding, pasando por la QFT sobre ℤ_N, hasta el análisis de probabilidad de éxito y el número esperado de repeticiones + simulador clásico de circuitos cuánticos de n qubits con complejidad O(4ⁿ poly(n)), validado factorizando un semiprimo pequeño.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del simulador y se declara su escalamiento respecto al número de qubits, contrastado contra la cota O(4ⁿ poly(n)) derivada. Es la ficha donde el escalamiento del costo es el resultado, no una nota al margen: fija el límite de *n* alcanzable con el presupuesto disponible.

**Bibliografía.**
- **Base:** *Quantum Computation and Quantum Information* — Nielsen & Chuang (edición aniversario)
- **Complementaria:** *Quantum Computing Since Democritus* — Aaronson · *Quantum Computation Lecture Notes* — Preskill (Caltech Ph219, gratuito)
- **Papers:** *"Polynomial-Time Algorithms for Prime Factorization..."* — Shor (SIAM J. Comput. 1997) · *"A Fast Quantum Mechanical Algorithm for Database Search"* — Grover (STOC 1996)

**Recursos.** MIT OCW 8.370 · theory.caltech.edu/~preskill/ph219 · Qiskit y Cirq para simulación · scottaaronson.blog para discusión crítica de afirmaciones de supremacía.

**Protocolo de estudio.** Cada algoritmo se simula clásicamente con n pequeño antes de razonar sobre n grande. El álgebra lineal de MAT-102 se recupera explícitamente aquí: es exactamente el mismo objeto matemático, y tratarlo como algo nuevo duplica el costo de aprendizaje.

---

