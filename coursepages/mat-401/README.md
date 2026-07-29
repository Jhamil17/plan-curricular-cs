### MAT-401 — Álgebra Lineal Numérica y Optimización — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-102, MAT-103 |
| **ADN institucional** | Stanford EE364A/B (Boyd) · MIT 18.085 |

**Competencia terminal.** Reconoce convexidad, formula el dual de un problema y deriva la tasa de convergencia de un método de primer orden.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Convexidad | Conjuntos y funciones convexas · Operaciones que preservan convexidad · Funciones conjugadas · Reconocimiento de problemas convexos disfrazados |
| 2 | 4–6 | Dualidad | Dualidad de Lagrange · Gap de dualidad · Dualidad fuerte y condición de Slater · Condiciones KKT · Complementary slackness · Interpretación económica |
| 3 | 7–9 | Métodos de primer orden | Descenso de gradiente: convergencia para funciones L-suaves y μ-fuertemente convexas · Momentum · Nesterov con análisis O(1/k²) · Descenso de coordenadas · Métodos proximales |
| 4 | 10–12 | Métodos de segundo orden e interior | Newton: convergencia cuadrática local · Cuasi-Newton (BFGS) · Barrera logarítmica · Punto interior primal-dual · Complejidad de iteración |
| 5 | 13–15 | Optimización estocástica y no suave | SGD: convergencia en esperanza · Varianza reducida (SVRG) · Norma-1: LASSO, Basis Pursuit · Subgradiente · Min-max y teorema minimax · Relajaciones LP/SDP en optimización combinatoria |

**Prueba de Dominio.** Demostración de que el método acelerado de Nesterov logra O(1/k²) frente a O(1/k) del gradiente estándar + implementación de un solver de programación cuadrática con restricciones de igualdad mediante multiplicadores de Lagrange, validado contra CVXPY.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del solver, con el escalamiento declarado respecto al número de variables y de restricciones. El número que decide algo es el **tamaño a partir del cual el sistema KKT denso deja de caber**: es la cantidad que en la práctica obliga a pasar a métodos que explotan estructura, y saberla convierte "usa un solver disperso" en una decisión derivada y no en un consejo heredado.

**Bibliografía.**
- **Base:** *Convex Optimization* — Boyd & Vandenberghe (gratuito)
- **Complementaria:** *Numerical Optimization* — Nocedal & Wright · *Lectures on Convex Optimization* — Nesterov · *First-Order Methods in Optimization* — Beck
- **Papers:** —

**Recursos.** web.stanford.edu/~boyd/cvxbook (libro + slides + video de EE364A) · CVXPY · MOSEK/ECOS para contrastar.

**Protocolo de estudio.** Asignatura puente hacia el ciclo VI. Cada resultado se etiqueta al aprenderlo con dónde reaparece en aprendizaje automático: KKT→SVM, dualidad→kernel trick, SGD→entrenamiento de redes. El etiquetado se hace ahora, no al llegar al ciclo VI.

---

