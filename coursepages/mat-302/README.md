### MAT-302 — Álgebra Abstracta para Computación

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-101 |
| **ADN institucional** | MIT 18.703 · UC Berkeley Math 113 |

**Competencia terminal.** Construye y opera en cuerpos finitos, y reconoce la estructura algebraica que subyace a un esquema criptográfico o a un código corrector.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Grupos | Axiomas, subgrupos, cocientes · Homomorfismos · Teoremas de isomorfía · Teorema de Lagrange · Grupos cíclicos |
| 2 | 4–6 | Acciones y permutaciones | Teorema de Cayley · Órbitas y estabilizadores · Lema de Burnside · Enumeración de Pólya · Grupos de simetría |
| 3 | 7–9 | Anillos | Dominio íntegro · Ideales y cocientes · Anillos de polinomios · Aritmética en ℤ/nℤ · φ de Euler · Pequeño teorema de Fermat |
| 4 | 10–12 | Cuerpos finitos | GF(p) y GF(pⁿ) · Polinomios irreducibles · Construcción de GF(2ⁿ) · Elemento primitivo · Aplicación a AES (MixColumns) y a Reed-Solomon |
| 5 | 13–15 | Galois y representaciones | Extensiones de cuerpos · Grupo de Galois · Correspondencia de Galois · Teoría de representaciones: Maschke, caracteres · Transformada de Fourier sobre grupos finitos |

**Prueba de Dominio.** Construcción formal de GF(2⁸) con aritmética de polinomios irreducibles, e implementación de MixColumns de AES verificada contra los vectores de prueba de FIPS 197 + demostración de que el orden del grupo de Galois de una extensión finita es igual a su grado sobre el cuerpo base.

**Bibliografía.**
- **Base:** *Abstract Algebra* (3ª ed.) — Dummit & Foote
- **Complementaria:** *Algebra* — Artin · *A Computational Introduction to Number Theory and Algebra* — Shoup (gratuito)
- **Estándar:** FIPS 197 (especificación de AES)

**Recursos.** shoup.net/ntb (libro completo gratuito) · SageMath para aritmética en cuerpos finitos · MIT OCW 18.703.

**Protocolo de estudio.** Cada estructura abstracta se ancla en dos instancias concretas: una criptográfica (que reaparece en SEG-701) y una de códigos (que reaparece en TEO-401). Sin el anclaje, el material no transfiere y se olvida entre ciclos.

---

