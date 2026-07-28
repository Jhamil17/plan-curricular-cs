### IAP-601 — Fundamentos Matemáticos del Aprendizaje Automático — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 11 · **17 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-104, MAT-401, ALG-401 |
| **ADN institucional** | Stanford CS229 · UC Berkeley CS189 — vertiente teórica |

**Competencia terminal.** Deriva cotas de generalización y demuestra la convergencia de los algoritmos de aprendizaje que usa.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Teoría del aprendizaje | Marco PAC: clase de concepto, complejidad muestral · Consistencia · Dimensión VC: shattering, teorema de Vapnik-Chervonenkis · Complejidad de Rademacher · Compensación sesgo-varianza formalizada |
| 2 | 4–6 | Modelos lineales | OLS y sus propiedades (Gauss-Markov, BLUE) · Regularización L1/L2 y su interpretación bayesiana · Regresión logística: MLE, gradiente, Hessiano · GLMs y familia exponencial |
| 3 | 7–9 | Métodos de kernel | SVM de margen duro y suave · Dualidad de Lagrange aplicada (conexión con MAT-401) · Truco del kernel · Teorema de Mercer · Kernels válidos: RBF, polinomial, Matérn · Procesos Gaussianos |
| 4 | 10–12 | Modelos generativos y latentes | Estimación no paramétrica: k-NN con análisis asintótico · Algoritmo EM con prueba de convergencia · Mezclas gaussianas · Modelos gráficos: redes bayesianas, campos aleatorios de Markov · Inferencia exacta vs aproximada |
| 5 | 13–15 | Inferencia aproximada y ensembles | Inferencia variacional: ELBO, mean-field · MCMC: Metropolis-Hastings, Gibbs, diagnóstico de convergencia · Boosting: AdaBoost con prueba de margen · Bagging · Gradient Boosting |

**Prueba de Dominio.** Demostración del teorema fundamental de la teoría PAC (cota de generalización vía dimensión VC) + derivación completa del dual del SVM con kernel + prueba de convergencia del algoritmo EM para mezclas gaussianas. Cada resultado instanciado numéricamente.

**Bibliografía.**
- **Base:** *Understanding Machine Learning: From Theory to Algorithms* — Shalev-Shwartz & Ben-David (gratuito)
- **Complementaria:** *The Elements of Statistical Learning* (2ª ed.) — Hastie, Tibshirani & Friedman (gratuito) · *Pattern Recognition and Machine Learning* — Bishop · *Probabilistic Machine Learning* — Murphy (gratuito)
- **Papers:** *"A Training Algorithm for Optimal Margin Classifiers"* — Boser, Guyon & Vapnik (COLT 1992)

**Recursos.** cs229.stanford.edu (notas y problem sets) · Berkeley CS189 · probml.github.io (Murphy, gratuito) · scikit-learn solo como referencia de contraste, nunca como implementación primaria.

**Protocolo de estudio.** Cada cota se instancia numéricamente: ¿cuántas muestras exige para ε = 0.05 y δ = 0.05? El número suele ser absurdamente grande, y esa es la lección — la teoría acota, no predice el comportamiento práctico.

---

