### MAT-301 — Teoría de Grafos y Combinatoria Avanzada

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-101, MAT-104 |
| **ADN institucional** | MIT 18.217 · CMU 21-701 |

**Competencia terminal.** Aplica el método probabilístico para demostrar existencia y deriva cotas exactas sobre estructuras combinatorias.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Conectividad y flujo | Teorema de Menger · Flujo máximo: Ford-Fulkerson, Edmonds-Karp, Push-Relabel · Algoritmo de Dinic con análisis exacto O(V²E) por grafos de nivel · Max-flow min-cut |
| 2 | 4–6 | Emparejamiento | Bipartito: teorema de Hall, Hopcroft-Karp O(E√V) · Emparejamiento general: algoritmo blossom de Edmonds · Teorema de Tutte |
| 3 | 7–9 | Coloración y planaridad | Número cromático · Cota de Brooks · Teorema de Vizing · Coloración de listas · Planaridad: Kuratowski-Wagner · Boyer-Myrvold · Genus y grafos en superficies |
| 4 | 10–12 | Método probabilístico | Primer y segundo momento · Lovász Local Lemma simétrico y asimétrico · Desaleatorización · Números de Ramsey · Cotas por conteo |
| 5 | 13–15 | Estructuras avanzadas | Grafos expanders: expansión de arista y de vértice, gap espectral · Polinomio de Tutte · Matroides: definición axiomática, teorema del greedy · Teorema de Szemerédi (enunciado) |

**Prueba de Dominio.** Demostración del Lovász Local Lemma en sus versiones simétrica y asimétrica, con aplicación a coloración de hipergrafos + demostración de que el algoritmo de Dinic es O(V²E) mediante análisis de fases con grafos de nivel.

**Bibliografía.**
- **Base:** *Graph Theory* (5ª ed.) — Diestel (gratuito para lectura en línea)
- **Complementaria:** *The Probabilistic Method* — Alon & Spencer · *Modern Graph Theory* — Bollobás
- **Papers:** *"A Constructive Proof of the General Lovász Local Lemma"* — Moser & Tardos (JACM 2010)

**Recursos.** diestel-graph-theory.com · MIT OCW 18.217 · NetworkX y SageMath para verificar construcciones sobre instancias pequeñas.

**Protocolo de estudio.** El método probabilístico se practica en formato "existencia sin construcción": demostrar que existe, luego intentar construirlo explícitamente y fracasar conscientemente. Esa asimetría entre existencia y construcción es el contenido real de la unidad 4.

---

