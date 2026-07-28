### MAT-102 — Álgebra Lineal Computacional — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 7/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | ∅ |
| **ADN institucional** | MIT 18.06 (Strang) |

**Competencia terminal.** Descompone matrices con control explícito del error numérico y traduce cada operación algebraica a su significado geométrico y a su costo computacional.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Espacios vectoriales | Espacios sobre campos arbitrarios · Independencia, base, dimensión · Transformaciones lineales y representación matricial · Los cuatro subespacios fundamentales |
| 2 | 4–6 | Eliminación y factorización | Eliminación Gaussiana · LU, PLU con pivoteo · Espacio nulo, rango, nulidad · Complejidad O(n³) |
| 3 | 7–9 | Ortogonalidad | Proyecciones ortogonales · Gram-Schmidt · QR · Mínimos cuadrados · Pseudoinversa de Moore-Penrose |
| 4 | 10–12 | Espectro | Valores y vectores propios · Diagonalización · Forma de Jordan · Descomposición espectral · Matrices simétricas y definidas positivas |
| 5 | 13–15 | SVD y estabilidad numérica | SVD y aplicaciones (compresión, PCA, rango bajo) · Normas matriciales · Número de condición · Estabilidad y error de redondeo |

**Prueba de Dominio.** Solver directo tipo LAPACK escrito desde cero en C para `Ax = b` con factorización LU y pivoteo parcial. Análisis de error numérico y verificación de la complejidad O(n³) por medición.

**Bibliografía.**
- **Base:** *Introduction to Linear Algebra* (6ª ed., 2023) — Strang
- **Complementaria:** *Numerical Linear Algebra* — Trefethen & Bau · *Matrix Computations* — Golub & Van Loan
- **Papers:** —

**Recursos.** MIT OCW 18.06 (curso completo en video, Strang) · MIT 18.065 (versión aplicada a datos) · Referencia BLAS/LAPACK para contrastar el solver propio.

**Protocolo de estudio.** Cada descomposición se ejecuta a mano sobre una matriz 3×3 antes de codificarla. La interpretación geométrica —qué le hace la transformación al espacio— se verbaliza en voz alta por operación, no por tema.

---

