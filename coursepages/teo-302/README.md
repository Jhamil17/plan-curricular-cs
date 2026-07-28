### TEO-302 — Teoría de la Complejidad Computacional — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 12 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | TEO-301 (concurrente permitido) |
| **ADN institucional** | UC Berkeley CS172 · MIT 6.1400[J] *(ex 6.045)* · MIT 6.5400 |

**Competencia terminal.** Clasifica problemas en clases de complejidad mediante reducción y distingue con precisión lo demostrado de lo conjeturado.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Clases de tiempo y espacio | TIME(f), SPACE(f) · P, NP, co-NP, PSPACE, EXPTIME · Definición por certificado y por máquina no determinista · Teoremas de jerarquía de tiempo y espacio |
| 2 | 4–6 | NP-completitud | Reducciones polinomiales (≤ₚ) · Teorema de Cook-Levin con demostración completa · Cadena canónica: SAT → 3-SAT → Clique → Independent Set → Vertex Cover → Hamiltonian Path |
| 3 | 7–9 | Espacio | Teorema de Savitch: NSPACE(f) ⊆ SPACE(f²) · Teorema de Immerman-Szelepcsényi · PSPACE-completitud: QBF/TQBF · L, NL y NL-completitud |
| 4 | 10–12 | Aleatoriedad y circuitos | BPP, RP, co-RP, ZPP · Teorema de Adleman: BPP ⊆ P/poly · Circuitos booleanos: tamaño y profundidad · NC y AC · Teorema de Valiant |
| 5 | 13–15 | Más allá de NP | Jerarquía polinomial · #P y Teorema de Toda · Complejidad de comunicación · Complejidad de consultas: certificado, sensibilidad, grado |

**Prueba de Dominio.** Demostración de Cook-Levin desde la codificación del cómputo como fórmula + demostración del Teorema de Savitch + construcción de la jerarquía polinomial mediante oráculos y análisis de su relación con P vs NP (incluyendo por qué la relativización obstruye ciertas técnicas de prueba).

**Bibliografía.**
- **Base:** *Computational Complexity: A Modern Approach* — Arora & Barak
- **Complementaria:** *Computational Complexity* — Papadimitriou · *The Nature of Computation* — Moore & Mertens
- **Papers:** *"The Complexity of Theorem-Proving Procedures"* — Cook (STOC 1971) · *"Relativizations of the P =? NP Question"* — Baker, Gill & Solovay (1975)

**Recursos.** Arora & Barak (borrador gratuito en la web de Princeton) · Complexity Zoo · Berkeley CS172 notes.

**Protocolo de estudio.** Mapa de clases dibujado de memoria cada semana, con las inclusiones **conocidas** en trazo continuo y las **conjeturadas** en trazo punteado. Confundir ambas es el fallo conceptual central de la asignatura y la causa de argumentos circulares en los exámenes.

---

