### ALG-403 — Computación Paralela y Distribuida

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | ALG-201, SIS-201 |
| **ADN institucional** | CMU 15-210 · Stanford CS149 · MIT 6.106 *(ex 6.172)* |

**Competencia terminal.** Analiza un algoritmo paralelo en términos de trabajo y span, y demuestra la linearizabilidad de una estructura concurrente.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelos de cómputo paralelo | PRAM: EREW, CREW, CRCW y simulaciones mutuas · Modelo Work-Span (Cilk) · Ley de Brent · Paralelismo = W/S · Amdahl y Gustafson |
| 2 | 4–6 | Algoritmos paralelos | Prefix sums (scan) · Mergesort paralelo · List ranking · BFS paralelo (PBFS) · Redes de ordenamiento: Batcher bitonic |
| 3 | 7–9 | Arquitectura de memoria compartida | UMA vs NUMA · Coherencia de caché: MSI, MESI, MOESI · False sharing y padding · Modelos de consistencia: sequential consistency, TSO, release consistency |
| 4 | 10–12 | Sincronización | Mutexes, semáforos, barreras, variables de condición · Lock-free y wait-free · CAS, LL/SC · ABA problem · Memoria transaccional: STM, HTM |
| 5 | 13–15 | Planificación y GPU | Work-stealing scheduler y su cota · OpenMP · Modelo de ejecución GPU: warps, divergencia, ocupancia · Introducción a CUDA |

**Prueba de Dominio.** Suma de prefijos paralela con análisis exacto de W(n) = O(n) y S(n) = O(log n), verificado por medición de escalabilidad + cola MPMC lock-free con demostración de linearizabilidad y con banco de pruebas de estrés bajo reordenamiento de memoria.

**Bibliografía.**
- **Base:** *The Art of Multiprocessor Programming* (2ª ed.) — Herlihy, Shavit, Luchangco & Spear
- **Complementaria:** *Introduction to Parallel Computing* — Kumar et al. · *Structured Parallel Programming* — McCool, Reinders & Robison
- **Papers:** *"Scheduling Multithreaded Computations by Work Stealing"* — Blumofe & Leiserson (JACM 1999) · *"Linearizability: A Correctness Condition for Concurrent Objects"* — Herlihy & Wing (TOPLAS 1990)

**Recursos.** CMU 15-210 · Stanford CS149 · MIT 6.106 · ThreadSanitizer, `perf`, Intel Inspector · Cilk / OpenCilk.

**Protocolo de estudio.** Todo argumento de correctitud concurrente se escribe primero como historia de ejecución con entrelazado explícito, antes de codificar. Los bugs de concurrencia no se depuran: se previenen en la especificación, porque no son reproducibles.

---

