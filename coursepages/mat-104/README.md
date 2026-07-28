### MAT-104 — Probabilidad y Procesos Estocásticos — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 10 · **16 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ∅ |
| **ADN institucional** | MIT 6.3700 *(ex 6.041)* · UC Berkeley EECS 126 · Harvard Stat 110 |

**Competencia terminal.** Analiza la complejidad esperada de algoritmos aleatorizados y modela sistemas con cadenas de Markov y teoría de colas.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Fundamentos medibles | Espacio de probabilidad (Ω, F, P) · σ-álgebras · Independencia · Probabilidad condicional · Bayes |
| 2 | 4–6 | Variables aleatorias | Discretas y continuas · Esperanza, varianza, momentos · Función generadora de momentos · Binomial, Poisson, Gaussiana, Exponencial |
| 3 | 7–9 | Teoremas límite | Desigualdades de Markov, Chebyshev, Chernoff · Ley de los grandes números (débil y fuerte) · Teorema Central del Límite con demostración |
| 4 | 10–12 | Procesos de Markov | Cadenas de Markov: clasificación de estados, ergodicidad, distribución estacionaria · Procesos de Poisson y renovación · Teoría de colas: M/M/1, M/G/1, redes de Jackson |
| 5 | 13–15 | Probabilidad en algoritmos | Monte Carlo vs Las Vegas · Hashing universal y aleatorizado · Análisis probabilístico de estructuras de datos · Concentración |

**Prueba de Dominio.** Análisis completo de la complejidad esperada del Quicksort aleatorizado + demostración de que las Skip Lists logran O(log n) en esperanza + análisis de Bloom Filters con derivación de la tasa óptima de falsos positivos. Cada resultado verificado por simulación.

**Bibliografía.**
- **Base:** *Introduction to Probability* (2ª ed.) — Blitzstein & Hwang (Harvard Stat 110)
- **Complementaria:** *Probability: Theory and Examples* — Durrett (nivel medida) · *Probability and Computing* — Mitzenmacher & Upfal
- **Papers:** —

**Recursos.** Harvard Stat 110 (video completo, gratuito) · MIT OCW 6.041 · UC Berkeley EECS 126 notes.

**Protocolo de estudio.** Toda cota se verifica por simulación antes de aceptarse. La discrepancia entre cota teórica y simulación es señal de error en la derivación, no ruido experimental.

---

