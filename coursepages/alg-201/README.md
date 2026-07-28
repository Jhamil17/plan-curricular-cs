### ALG-201 — Estructuras de Datos Fundamentales — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–2–2 / 9 · **16 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-101, MAT-104, SIS-101 |
| **ADN institucional** | MIT 6.1210 *(ex 6.006)* · CMU 15-210 |

**Competencia terminal.** Deriva cotas amortizadas con función potencial y selecciona estructuras a partir del análisis, no del repertorio memorizado.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Análisis amortizado | Método agregado, del banquero y del potencial · Arrays dinámicos · Contador binario · Tablas dinámicas con contracción |
| 2 | 4–6 | Árboles balanceados | BST · AVL con demostración de altura O(log n) · Rojo-Negro · Rotaciones y aumentación · B-Trees y B+-Trees para disco |
| 3 | 7–9 | Colas de prioridad | Heaps binarios y d-heaps · Fibonacci heaps: análisis amortizado de decrease-key con función potencial · Pairing heaps |
| 4 | 10–12 | Hashing | Encadenamiento vs open addressing · Hashing universal y perfecto · Cuckoo · Robin Hood · Análisis probabilístico de colisiones |
| 5 | 13–15 | Estructuras especializadas | Tries y Patricia tries · Árboles de segmento y Fenwick (BIT) · Disjoint-Set Union con union-by-rank y path compression (inversa de Ackermann) · Skip lists · van Emde Boas |

**Prueba de Dominio.** Demostración formal de que las operaciones de Fibonacci Heap son O(1) amortizado (extract-min O(log n)) mediante función potencial de Fibonacci, e implementación desde cero con medición que contraste la cota amortizada contra el peor caso individual.

**Bibliografía.**
- **Base:** *Introduction to Algorithms* (4ª ed., 2022) — Cormen, Leiserson, Rivest & Stein (CLRS)
- **Complementaria:** *Advanced Data Structures* — Brass · *Purely Functional Data Structures* — Okasaki
- **Papers:** *"Fibonacci Heaps and Their Uses in Improved Network Optimization Algorithms"* — Fredman & Tarjan (JACM 1987)

**Recursos.** MIT OCW 6.006 y 6.851 (Advanced Data Structures, Demaine) · UC Berkeley CS61B · Visualizadores: visualgo.net.

**Protocolo de estudio.** Cada estructura se implementa una vez y se **reimplementa a los 30 días desde cero**, sin mirar la versión previa. La segunda implementación es la que cuenta para la evaluación.

---

