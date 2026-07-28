### ALG-801 — Complejidad Fina y Algoritmos de Frontera

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 12 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ALG-402, TEO-302 |
| **ADN institucional** | MIT 6.890 *(R. Williams & V. Vassilevska Williams)* · UC Berkeley CS294 |

**Competencia terminal.** Demuestra cotas inferiores condicionadas y sitúa un problema dentro del grafo de hipótesis de complejidad fina.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Hipótesis y reducciones finas | SETH y ETH · Orthogonal Vectors Conjecture · 3-SUM hardness · APSP-equivalencias · Reducciones que preservan el exponente |
| 2 | 4–6 | Cotas inferiores condicionadas | SETH-hardness de Edit Distance, LCS, Fréchet distance · Consecuencias para problemas de cadenas y de grafos · Barreras a la mejora de exponentes |
| 3 | 7–9 | Dureza de aproximación | Teorema PCP: enunciado y construcción · Long Code · Reducciones gap-introducing · Clique (no n^(1−ε)) · Set Cover (ln n ajustado) · Unique Games Conjecture y sus implicaciones para Vertex Cover y Max-Cut |
| 4 | 10–12 | Algoritmos para datos masivos | Streaming: Morris, Flajolet-Martin, AMS sketch · Count-Min · Johnson-Lindenstrauss y reducción de dimensión · Property testing: ε-tester y complejidad de consultas · Algoritmos sublineales |
| 5 | 13–15 | Tratabilidad parametrizada y complejidad algebraica | FPT y jerarquía W · Treewidth y DP sobre descomposición arbórea · Kernelización y cotas inferiores de kernel · Circuitos aritméticos · Permanent vs Determinant (Valiant) · Strassen y cotas inferiores de multiplicación de matrices |

**Prueba de Dominio.** Demostración formal de que Edit Distance no admite algoritmo de tiempo O(n^(2−ε)) salvo que SETH sea falsa, con la reducción explícita desde OV + construcción completa de un PCP para un lenguaje NP-completo con gap 1/2.

**Bibliografía.**
- **Base:** *Computational Complexity: A Modern Approach* — Arora & Barak
- **Complementaria:** *Parameterized Algorithms* — Cygan et al. (gratuito) · *The Probabilistic Method* — Alon & Spencer
- **Papers:** *"Fine-Grained Algorithms and Complexity"* (survey) — Vassilevska Williams · *"Edit Distance Cannot Be Computed in Strongly Subquadratic Time"* — Backurs & Indyk (STOC 2015) · *"Probabilistic Checking of Proofs"* — Arora & Safra (JACM 1998)

**Recursos.** MIT 6.890 (notas públicas) · people.csail.mit.edu/virgi (surveys y slides) · ECCC (Electronic Colloquium on Computational Complexity) para papers recientes.

**Protocolo de estudio.** Cada reducción se dibuja como nodo en un diagrama de dependencias condicionales. La estructura del campo **es** ese grafo; memorizar resultados aislados sin la estructura no permite ni reconocer ni construir reducciones nuevas.

---

