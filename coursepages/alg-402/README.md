### ALG-402 — Algoritmos Avanzados y Geometría Computacional

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 12 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ALG-401 (concurrente permitido) |
| **ADN institucional** | MIT 6.5210[J] / 18.415[J] *(ex 6.854, Karger)* · Stanford CS261 |

**Competencia terminal.** Deriva razones de aproximación ajustadas y construye la instancia que las alcanza.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Flujo avanzado y LP | Scaling algorithms · Min-cost flow · Programación lineal: simplex, dualidad débil y fuerte · Teorema de Farkas · Método del elipsoide · Relajaciones LP con redondeo |
| 2 | 4–6 | Aproximación | Razón de aproximación · PTAS y FPTAS · Set Cover greedy con cota ln(n) e instancia ajustada · Vertex Cover 2-aproximación · Christofides (3/2) para TSP métrico · Relajaciones SDP: Goemans-Williamson |
| 3 | 7–9 | Aleatorización y online | Fingerprinting · Freivalds · Karger min-cut con análisis de probabilidad de éxito · Análisis competitivo · Método del potencial · Problema del k-servidor · Paging online |
| 4 | 10–12 | Geometría computacional | Triangulación · Diagramas de Voronoi (algoritmo de Fortune) · Delaunay · Sweep line · Intersección de semiplanos · Búsqueda de rango |
| 5 | 13–15 | Memoria externa y cadenas | External memory: B-trees, sorting, scanning · Cache-oblivious: multiplicación de matrices, funnelsort · Suffix arrays con SA-IS · FM-index · Compresión con Burrows-Wheeler |

**Prueba de Dominio.** Implementación del algoritmo de Karger con análisis riguroso de la probabilidad de éxito y del número de repeticiones necesarias + demostración de la dualidad fuerte de la programación lineal mediante el Teorema de Farkas.

**Bibliografía.**
- **Base:** *Randomized Algorithms* — Motwani & Raghavan
- **Complementaria:** *The Design of Approximation Algorithms* — Williamson & Shmoys (gratuito) · *Computational Geometry: Algorithms and Applications* — de Berg et al. · *Approximation Algorithms* — Vazirani
- **Papers:** *"Improved Approximation Algorithms for Maximum Cut..."* — Goemans & Williamson (JACM 1995) · *"Global Min-cuts in RNC..."* — Karger & Stein

**Recursos.** designofapproxalgs.com (libro gratuito) · MIT 6.5210 (notas de Karger) · Stanford CS261 · CGAL para contrastar implementaciones geométricas.

**Protocolo de estudio.** Para cada algoritmo de aproximación se construye la instancia que alcanza la cota ajustada. Sin esa instancia, la cota es un número memorizado y no se entiende por qué el algoritmo no puede hacerlo mejor.

---

