### MAT-101 — Matemáticas Discretas y Lógica Formal — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 10 · **16 h/sem** |
| **Dificultad** | 7/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ∅ |
| **ADN institucional** | MIT 6.1200[J] *(ex 6.042)* · UC Berkeley CS70 |

**Competencia terminal.** Construye demostraciones formales por inducción estructural, contradicción y construcción directa, y detecta el punto exacto donde una demostración incorrecta falla.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Lógica y método de prueba | Lógica proposicional · Lógica de primer orden · Deducción natural · Teoría de pruebas · Prueba directa, contrapositiva, contradicción · Errores de cuantificación |
| 2 | 4–6 | Fundamentos de conjuntos | Teoría axiomática ZFC · Relaciones, funciones, órdenes parciales · Cardinalidad · Diagonalización de Cantor |
| 3 | 7–9 | Inducción | Inducción débil, fuerte y estructural · Recursión bien fundada · Invariantes de estado · Terminación |
| 4 | 10–12 | Teoría de números | Aritmética modular · MCD y Euclides extendido · Inversos modulares · Teorema Chino del Resto · Generadores · Logaritmo discreto |
| 5 | 13–15 | Grafos y combinatoria | Conectividad, árboles, coloración, planaridad · Permutaciones y combinaciones · Principio de inclusión-exclusión · Funciones generatrices |

**Prueba de Dominio.** Demostración formal, desde axiomas ZFC, de la correctitud del algoritmo de Euclides extendido. Construcción de un solucionador SAT por resolución proposicional con prueba de terminación y análisis de complejidad empírica contrastada contra la cota teórica.

**Contabilidad de costo (§15.8).** Se cuentan las operaciones de resolución del solucionador y se declara su escalamiento respecto al número de variables y cláusulas, contrastado contra la complejidad derivada. El número que decide algo es dónde la razón cláusulas/variables hace que el costo explote: fija el tamaño de instancia con el que se puede trabajar y conecta con el umbral de fase que INT-100 estudia. **Sin componente de memoria:** la huella se exige solo donde el plan ya entregó la jerarquía de memoria (§15.2), que aquí sería inversión de prerrequisitos.

**Bibliografía.**
- **Base:** *Mathematics for Computer Science* — Lehman, Leighton & Meyer (MIT, gratuito)
- **Complementaria:** *Discrete Mathematics and Its Applications* — Rosen · *How to Prove It* — Velleman
- **Papers:** —

**Recursos.** MIT OCW 6.042J (video completo + problem sets con solución) · Berkeley CS70 notes · Automata Tutor · Lean 4 para verificar pruebas de la unidad 3.

**Protocolo de estudio.** Toda demostración se reconstruye desde el enunciado en blanco a los 3, 10 y 30 días. Es la asignatura donde el tipo de tarjeta *punto de quiebre* rinde más: para cada teorema, una tarjeta por hipótesis eliminada.

---

