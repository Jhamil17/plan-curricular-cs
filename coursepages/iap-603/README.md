### IAP-603 — Inteligencia Artificial: Búsqueda, Planificación y Razonamiento

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-104, ALG-401 |
| **ADN institucional** | UC Berkeley CS188 · Stanford CS221 — vertiente teórica |

**Competencia terminal.** Demuestra propiedades de optimalidad y convergencia de agentes de búsqueda y de aprendizaje por refuerzo.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Búsqueda | BFS, DFS, costo uniforme · A*: admisibilidad, consistencia, completitud y optimalidad con demostración · IDA*, RBFS, SMA* · Diseño de heurísticas y dominancia |
| 2 | 4–6 | Búsqueda adversarial | Minimax · Poda alfa-beta con análisis del factor de ramificación efectivo · Expectimax · MCTS y UCT con la cota de confianza superior |
| 3 | 7–9 | Satisfacción de restricciones | CSP · Backtracking con heurísticas de orden · Arc consistency (AC-3) · Forward checking · Búsqueda local: GSAT, WalkSAT · Planificación: STRIPS, PDDL, orden parcial |
| 4 | 10–12 | Razonamiento probabilístico | Redes bayesianas · Inferencia exacta por eliminación de variables · Belief propagation · HMM: forward-backward, Viterbi, Baum-Welch como caso de EM |
| 5 | 13–15 | Decisión y refuerzo | MDP · Ecuaciones de Bellman · Value iteration y policy iteration con prueba de convergencia por contracción · Q-learning con análisis de convergencia · TD y SARSA · Policy gradient: REINFORCE, Actor-Critic, PPO |

**Prueba de Dominio.** Demostración formal de la optimalidad de A* con heurística admisible y consistente, incluyendo el contraejemplo que muestra por qué la admisibilidad sola no basta para grafos + agente de Q-learning con convergencia demostrada al óptimo en un MDP finito donde el óptimo se calcula en forma cerrada.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del agente, con el escalamiento declarado respecto al tamaño del espacio de estados y acciones. El número que decide algo es el **umbral donde la tabla deja de caber y el número de episodios deja de ser alcanzable**: es exactamente lo que motiva la aproximación de funciones, y encontrarlo por medición convierte esa transición en una decisión derivada en lugar de un dogma heredado.

**Bibliografía.**
- **Base:** *Artificial Intelligence: A Modern Approach* (4ª ed.) — Russell & Norvig
- **Complementaria:** *Reinforcement Learning: An Introduction* (2ª ed.) — Sutton & Barto (gratuito) · *Algorithms for Decision Making* — Kochenderfer et al. (gratuito)
- **Papers:** *"Bandit Based Monte-Carlo Planning"* — Kocsis & Szepesvári (ECML 2006)

**Recursos.** inst.eecs.berkeley.edu/~cs188 (proyectos Pacman) · incompleteideas.net/book (Sutton & Barto gratuito) · algorithmsbook.com · Gymnasium para entornos.

**Protocolo de estudio.** Toda propiedad de convergencia se verifica empíricamente en un entorno de juguete donde el óptimo es calculable en forma cerrada. Sin ese contraste no hay verificación: hay confianza en que el código está bien.

---

