### ALG-401 — Diseño y Análisis de Algoritmos — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ALG-201, MAT-104 |
| **ADN institucional** | MIT 6.1220[J] / 18.410[J] *(ex 6.046)* |

**Competencia terminal.** Diseña un algoritmo para un problema no visto, enuncia su invariante, demuestra su correctitud y deriva su complejidad exacta.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Divide y vencerás | Recurrencias · Teorema Maestro con demostración · Método de Akra-Bazzi · Mergesort, heapsort · Cota inferior Ω(n log n) por árbol de decisión · Selección determinista |
| 2 | 4–6 | Programación dinámica | Subestructura óptima · Solapamiento de subproblemas · Memoización vs bottom-up · LCS, LIS, Edit Distance, Knapsack, Matrix Chain · Reconstrucción de la solución |
| 3 | 7–9 | Greedy y matroides | Correctitud por exchange argument · Matroides y el teorema del greedy · Huffman · Scheduling · Cuándo greedy falla y por qué |
| 4 | 10–12 | Algoritmos de grafos | Dijkstra con Fibonacci heaps O(E + V log V) · Bellman-Ford · Floyd-Warshall · MST: Kruskal con DSU, Prim · SCC: Tarjan, Kosaraju · Flujo y matching |
| 5 | 13–15 | Geometría y cadenas | Convex hull: Graham, Jarvis · Intersección de segmentos por sweep line · KMP, Z-algorithm, Aho-Corasick · Suffix arrays y suffix trees |

**Prueba de Dominio.** Demostración de correctitud de Dijkstra mediante invariante de bucle, con análisis exacto usando Fibonacci heaps + demostración de que Knapsack 0/1 no admite solución greedy pero la versión fraccionada sí, con el exchange argument explícito y el contraejemplo mínimo para la versión entera.

**Bibliografía.**
- **Base:** CLRS (4ª ed.) + *Algorithm Design* — Kleinberg & Tardos
- **Complementaria:** *Algorithms* — Dasgupta, Papadimitriou & Vazirani (gratuito) · *Competitive Programming* — Halim (para volumen de práctica)
- **Papers:** —

**Recursos.** MIT OCW 6.046J · Stanford Algorithms Specialization (Roughgarden) · Codeforces y AtCoder para práctica cronometrada · Stanford CS161.

**Protocolo de estudio.** Formato de tarjeta canónico: problema → **invariante**, nunca problema → pseudocódigo. Un algoritmo memorizado sin su invariante no está aprendido. Práctica diaria obligatoria: un problema no visto, cronometrado a 45 minutos.

---

