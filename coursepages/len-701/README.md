### LEN-701 — Tipos Dependientes y Verificación Mecanizada

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–2–2 / 10 · **17 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | LEN-201, LEN-502, TEO-303 |
| **ADN institucional** | CMU 15-317 y 15-819 · MIT 6.826 |

**Competencia terminal.** Expresa una especificación como tipo y produce un programa cuya corrección es consecuencia de que tipa.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Curry-Howard extendida | Proposiciones como tipos, pruebas como programas · Lógica intuicionista vs clásica · Sistema F: polimorfismo de segundo orden, normalización fuerte · Parametricidad (Reynolds) |
| 2 | 4–6 | Tipos dependientes | Π-tipos y Σ-tipos · Tipo identidad · Teoría de tipos de Martin-Löf · Universos y su jerarquía · Cálculo de Construcciones · Sort checking |
| 3 | 7–9 | Asistentes de prueba | Lean 4 y su biblioteca mathlib · Rocq (antes Coq) · Tácticas y procedimientos de decisión · Reflexión por cómputo · Extracción de código certificado |
| 4 | 10–12 | Teoría de tipos homotópica | Igualdad como camino · Axioma de univalencia · Tipos inductivos superiores · Interpretación de los tipos como espacios · Consecuencias para el razonamiento sobre estructuras |
| 5 | 13–15 | Sistemas de tipos aplicados | Refinement types: Liquid Haskell, subtipado con SMT · Efectos algebraicos y handlers · Free monads · Session types: protocolos como tipos · Sistemas subestructurales: lineales, afines, relevantes · Rust como sistema afín en producción |

**Prueba de Dominio.** Formalización completa en Lean 4 (o Rocq) de la correctitud de mergesort, incluyendo preservación de contenido (permutación) y de orden, con extracción de código ejecutable certificado y verificación de que el código extraído se comporta como el especificado.

**Bibliografía.**
- **Base:** *Software Foundations* Vol. 1–3 — Pierce et al. (gratuito)
- **Complementaria:** *Homotopy Type Theory: Univalent Foundations of Mathematics* — The Univalent Foundations Program (gratuito) · *Mathematics in Lean* (mathlib, gratuito) · *Certified Programming with Dependent Types* — Chlipala (gratuito) · *Practical Foundations for Programming Languages* — Harper
- **Papers:** *"Propositions as Types"* — Wadler (CACM 2015)

**Recursos.** softwarefoundations.cis.upenn.edu · leanprover-community.github.io · homotopytypetheory.org/book · Zulip de Lean para consultas · Agda y Idris 2 como alternativas de exploración.

**Protocolo de estudio.** Toda formalización arranca por el **enunciado del tipo**, antes que por la prueba. Si el tipo está mal formulado, la prueba es irrelevante — y un tipo mal planteado que sin embargo tipa es el error dominante y el más difícil de detectar de esta asignatura.

---

