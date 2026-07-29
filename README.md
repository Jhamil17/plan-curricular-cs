# Ciencias de la Computación — Programa de Rigor Extendido

🎓 Currículo autodiseñado de nivel bachiller + licenciatura en Ciencias de la Computación, con orientación a teoría, sistemas y métodos formales. Versión **2026.3**.

Este repositorio replica el formato de [ossu/computer-science](https://github.com/ossu/computer-science) — índice navegable con una ficha (README propio) por asignatura, tabla de prerrequisitos y changelog versionado — pero con contenido, metodología y sistema de evaluación propios. No es una copia del currículo de OSSU; ver [`RESOURCES.md`](RESOURCES.md) para dónde sí se apoya en cursos de OSSU y otras fuentes abiertas.

---

# PLAN CURRICULAR
## Ciencias de la Computación — Programa de Rigor Extendido
### Versión 2026.3

---

## Nota de la revisión 2026.3

Esta versión corrige un defecto de los criterios de evaluación. No añade contenido, no crea asignaturas y no altera la carga horaria: las 47 unidades, los 201 créditos y las ≈11 300 horas de la 2026.2 quedan idénticos.

**El defecto.** El plan evaluaba sistemas distribuidos y núcleos sin exigir que fueran observables, y proyectos de cómputo ejecutable sin exigir que su costo en recursos estuviera acotado. Dicho de otro modo: una Prueba de Dominio podía aprobarse demostrando que el artefacto *funciona*, sin poder decir a qué latencia, con qué tasa de error, contra qué recurso saturado ni a qué costo. Para un plan cuyas competencias C3 y C4 son precisamente razonar cuantitativamente sobre sistemas, eso es un hueco en el instrumento de evaluación, no una omisión de temario.

**La corrección.** Dos criterios nuevos en §15, que es donde vive el protocolo de Pruebas de Dominio: **§15.7 instrumentación obligatoria** —criterio-compuerta en SIS-501 y SIS-701, sujeto a la regla de no compensación de §6— y **§15.8 contabilidad de costo**, redactado como principio general y aplicado a las 22 fichas cuyo entregable es un programa cuyo costo crece con el tamaño de la entrada. La lista de las 22 se deriva del criterio y es re-derivable; las 17 que quedan fuera, la excepción de ALG-402 y el pendiente declarado de LEN-502 están en §15.2 con su motivo. Cada párrafo de ficha nombra la cantidad concreta que cierra una decisión de diseño: un criterio de costo que solo produce tablas de medición que nadie usa para decidir es contabilidad ritual, y §17 ya declara la presunción contra las prácticas que se sienten productivas sin serlo.

**Lo que no cambió.** Ninguna tabla de carga, créditos o horas: §3.2, §3.3, §4.1, §26 y §29 están intactos y siguen siendo recalculables desde las fichas. Las unidades semanales de las 47 fichas tampoco cambian. Lo único que se añadió a las fichas es el criterio de evaluación que les faltaba.

---

> Las notas de revisiones anteriores están archivadas en el §37 de [`CHANGELOG.md`](CHANGELOG.md), según la convención de notas de revisión de [`CONTRIBUTING.md`](CONTRIBUTING.md). La nota de la 2026.2 —que documenta el error de 1.7× en el presupuesto de horas y su corrección— está en §37.1.

---

# PARTE I — MARCO INSTITUCIONAL

## 1. Identificación del programa

| Campo | Valor |
|---|---|
| Denominación | Ciencias de la Computación |
| Grado | Bachiller en Ciencias de la Computación |
| Título | Licenciado en Ciencias de la Computación |
| Contenido | 8 ciclos de contenido (unidades de dependencia, no de calendario — ver §3.3) |
| Créditos totales | 201 (197 con ficha + 4 de optativa) |
| Asignaturas | 39 + 7 laboratorios integradores + 1 optativa = **47 unidades** |
| Carga total | **≈11 300 horas** de trabajo del estudiante (§3.2) |
| Régimen | Ciclos de 16 semanas de contenido; duración calendario según ruta (§14) |
| Modalidad | Presencial intensiva / autodidacta estructurada |

**Referencia curricular.** Cada asignatura declara su ADN institucional: el curso real de MIT, CMU, Stanford o UC Berkeley del que deriva su alcance y nivel de exigencia. No se trata de inspiración temática — el alcance, la profundidad demostrativa y el proyecto terminal replican el curso fuente.

**Exclusión declarada.** El programa no contiene asignaturas de ingeniería de software comercial, gestión de proyectos, DevOps, infraestructura como código, desarrollo web/móvil, emprendimiento ni habilidades blandas. Ver §34.

**Advertencia de calibración.** Este plan describe un programa cuya carga total equivale a **1.6–1.9 licenciaturas europeas de 240 ECTS** (§3.2). Presentarlo como una carrera de cuatro años sería falso. Las rutas de §14 son la forma honesta de recorrerlo, y la ruta que el documento recomienda por defecto no es la completa.

---

## 2. Perfil de egreso

Competencias verificables. Cada una está anclada a asignaturas específicas y se evidencia en artefactos evaluables, no en declaraciones de intención.

| # | Competencia terminal | Evidencia | Asignaturas |
|---|---|---|---|
| C1 | Construye demostraciones formales correctas y detecta fallos en demostraciones ajenas | Pruebas escritas de Cook-Levin, FLP, Gödel I, Nyquist-Shannon, LLL | MAT-101, TEO-302, TEO-303, MAT-301 |
| C2 | Diseña algoritmos con análisis exacto de complejidad y prueba de correctitud vía invariante | Análisis amortizado, cotas ajustadas, instancias de peor caso | ALG-201, ALG-401, ALG-402, ALG-801 |
| C3 | Implementa sistemas de bajo nivel desde cero con gestión explícita de recursos | Kernel, compilador, motor DBMS, procesador RISC-V | SIS-101, SIS-201, SIS-501, LEN-501, SIS-503 |
| C4 | Razona sobre concurrencia y distribución con modelos formales de consistencia y falla | Raft verificado, estructuras lock-free linearizables | ALG-403, SIS-701 |
| C5 | Deriva y verifica resultados de aprendizaje automático desde sus fundamentos matemáticos | Cota VC, dual SVM, backprop analítico, leyes de escalamiento | IAP-601, IAP-602, IAP-801, MAT-401 |
| C6 | Construye y evalúa argumentos de seguridad como reducciones formales | Protocolo Σ con simulación, exploit ROP, prueba IND-CCA2 | SEG-701, SEG-702 |
| C7 | Especifica y verifica programas con métodos formales mecanizados | Formalización en Lean 4 / Rocq, model checking LTL | LEN-201, LEN-502, LEN-701 |
| C8 | Lee críticamente literatura primaria, replica resultados y produce investigación original | 2 replicaciones + paper original + tesis defendida | INV-801, INV-802 |
| C9 | Gestiona su propio aprendizaje con instrumentación medible y calibración honesta | Bitácora fechada, serie de error de calibración, ajuste documentado del método | Transversal (§8–§18) |

**Sobre C9.** Es nueva en esta versión y es transversal, no una asignatura. Se incluye porque una ruta de 5+ años se sostiene o se cae por la capacidad de medir el propio rendimiento sin autoengaño, y porque es la única competencia del perfil que sigue rindiendo después de que el contenido específico se desactualice. Se evidencia en la serie temporal de error de calibración (§14.3), no en una declaración.

---

## 3. Sistema de créditos, carga y presupuesto de horas

### 3.1 Definición de crédito

**Definición legal (compatibilidad institucional).** 1 crédito = 16 horas lectivas teóricas o 32 horas lectivas prácticas por ciclo de 16 semanas. Es la definición del sistema peruano y la que usan las fichas.

**Notación de carga.** Cada asignatura declara `T–P–L / EI`:

| Sigla | Significado |
|---|---|
| **T** | Horas de teoría por semana |
| **P** | Horas de práctica dirigida por semana |
| **L** | Horas de laboratorio por semana |
| **EI** | Horas de estudio independiente por semana (no generan crédito, pero son obligatorias y están calendarizadas) |

**Ejemplo de lectura.** `MAT-101 · 5 créditos · 4–2–0 / 10` = 4 h teoría, 2 h práctica, 0 h laboratorio, 10 h estudio independiente = **16 h/semana**.

**Limitación conocida de la definición legal.** El crédito peruano cuenta solo horas lectivas e ignora el estudio independiente. Como en este programa el EI es el 60–70% del trabajo real, el número de créditos **subestima sistemáticamente la carga**. Por eso el documento usa además una segunda unidad, no negociable con la anterior:

**Definición de carga real (ECTS-equivalente).** 1 ECTS = 25–30 horas de trabajo total del estudiante, incluyendo lectivas, estudio independiente y evaluación. Es la unidad que permite comparar este programa con cualquier otro.

**Excepción declarada.** INV-801 e INV-802 (investigación y tesis) declaran créditos por carga total, no por horas lectivas: bajo la definición legal estricta, una tesis de 26 h/semana de trabajo mayoritariamente autónomo computaría 3 créditos, lo cual es absurdo. Se les asigna 4 y 8 créditos respectivamente por volumen de trabajo, siguiendo la práctica estándar. Es la única excepción del plan y se señala en lugar de disimularse.

### 3.2 Presupuesto real de horas

Suma directa de las 46 fichas de la Parte III, más la optativa estimada. Estas cifras son recalculables: se derivan del campo `Carga` de cada ficha.

| Ciclo de contenido | Fichas | Créditos | h lectivas/sem | h EI/sem | **h/sem total** | h del ciclo (×16) |
|---|---|---|---|---|---|---|
| I | 6 | 25 | 32 | 52 | **84** | 1 344 |
| II | 6 | 25 | 34 | 52 | **86** | 1 376 |
| III | 6 | 25 | 31 | 57 | **88** | 1 408 |
| IV | 6 | 25 | 32 | 56 | **88** | 1 408 |
| V | 6 | 25 | 35 | 56 | **91** | 1 456 |
| VI | 6 | 25 | 32 | 56 | **88** | 1 408 |
| VII | 6 | 25 | 35 | 54 | **89** | 1 424 |
| VIII | 4 + optativa | 26 | 23 + 5 | 55 + 9 | **92** | 1 472 |
| **Total** | **47** | **201** | — | — | — | **≈11 300 h** |

**Lectura obligatoria de esta tabla.** La columna `h/sem total` **no es un régimen propuesto**: es lo que costaría cursar los seis ítems de un ciclo en simultáneo. Nadie puede sostener 88 h/semana durante 128 semanas. La tabla existe para fijar el numerador —11 300 horas de contenido— y dejar que §14 elija el denominador.

### 3.3 Calibración externa

| Referencia | Horas totales | Este programa equivale a |
|---|---|---|
| Licenciatura europea estándar (240 ECTS) | ≈6 000–7 200 h | **1.6–1.9 licenciaturas** |
| Bachelor's estadounidense (120 credit hours × 45 h) | ≈5 400 h | **2.1 bachelor's** |
| Núcleo de este plan (§14.4, 27 unidades) | ≈6 480 h | **≈1 licenciatura completa** |
| Ruta de admisión a posgrado (§14.5, 12 unidades) | ≈3 150 h | **≈0.5 licenciatura** |

En ECTS-equivalente el programa completo es de **377–452 ECTS**. La cifra explica sola por qué no cabe en cuatro años: no hay defecto de diseño en el contenido, hay un error de rotulado en la duración. Un plan de 400 ECTS es un pregrado más un máster, no un pregrado.

### 3.4 El ciclo como unidad de dependencia, no de calendario

En la 2026.1 "ciclo" significaba dos cosas a la vez: un bloque de contenido con prerrequisitos resueltos y un semestre de 16 semanas de reloj. Confundirlas es lo que producía la aritmética imposible.

En esta versión se separan:

- **Ciclo de contenido (I–VIII).** Unidad lógica. Define qué se puede cursar cuándo, vía el grafo de §5. Es invariante entre rutas.
- **Bloque de calendario.** Unidad de reloj. Su duración depende de la ruta elegida en §14 y de las horas semanales disponibles reales.

Consecuencia práctica: **el orden de §4.2 y §5 se respeta siempre; la velocidad la fija §14.** Un estudiante en ruta R3 sigue exactamente la misma secuencia de dependencias que uno en R1, solo que el "Ciclo III" le toma 32 semanas de calendario en vez de 16.

### 3.5 Picos y semanas de sobrecarga

Con cualquier ruta, tres semanas por bloque concentran carga: la de Evaluación Parcial 1, la de Evaluación Parcial 2 y la de entrega de Prueba de Dominio. El incremento típico es de **+30–40% sobre la carga base** de la ruta.

**Regla dura.** El pico se absorbe reduciendo tarjetas nuevas (§12) y trabajo autónomo de otras asignaturas, **nunca reduciendo sueño**. La justificación no es de estilo de vida: es que la privación de sueño degrada la codificación hipocampal del material nuevo del día siguiente (§10.2), de modo que las horas ganadas se pagan con material que no se fija. Es una operación de pérdida neta y está documentada como tal.

---

## 4. Estructura de la malla

### 4.1 Áreas curriculares

Cifras verificadas contra las fichas de la Parte III. La columna `h totales` es la suma del campo `Carga` × 16 semanas.

| Código | Área | Unidades | Créditos | h totales | % del programa |
|---|---|---|---|---|---|
| **MAT** | Matemáticas para la computación | 8 | 36 | 1 952 | 17.3% |
| **SIS** | Sistemas y arquitectura | 9 | 40 | 2 304 | 20.4% |
| **TEO** | Teoría de la computación | 5 | 23 | 1 264 | 11.2% |
| **ALG** | Algoritmos y estructuras de datos | 5 | 24 | 1 328 | 11.8% |
| **LEN** | Lenguajes, compiladores y métodos formales | 4 | 19 | 1 040 | 9.2% |
| **IAP** | Inteligencia artificial y aprendizaje | 4 | 19 | 1 072 | 9.5% |
| **SEG** | Seguridad y criptografía | 2 | 9 | 512 | 4.5% |
| **INV** | Investigación | 2 | 12 | 672 | 5.9% |
| **INT** | Laboratorios integradores | 7 | 15 | 928 | 8.2% |
| **OPT** | Optativa de profundización | 1 | 4 | ≈224 | 2.0% |
| **Total** | | **47** | **201** | **≈11 300** | 100% |

**Corrección respecto de 2026.1.** La tabla anterior declaraba 47 asignaturas y 229 créditos; ambas cifras eran incorrectas. LEN figuraba con 5 asignaturas cuando tiene 4 (LEN-201, LEN-501, LEN-502, LEN-701), y los créditos por área estaban inflados en un 16% agregado. Las cifras de arriba se derivan de las fichas y se pueden reverificar sumando el campo `Créditos` de cada una.

**Lectura de la distribución.** SIS + MAT concentran el 37.7% del programa. Es deliberado: sistemas y matemáticas son las dos áreas donde el conocimiento no se desactualiza y donde la deuda técnica de aprendizaje es más cara de pagar después. IAP es solo el 9.5% pese a ser el área de mayor interés actual, por la razón declarada en §34: los fundamentos duran, la ingeniería sobre modelos tiene vida media de 18 meses.

### 4.2 Mapa de la malla

Orden de dependencia. La velocidad de recorrido la fija §14, no esta tabla.

```
CICLO I          CICLO II         CICLO III        CICLO IV
Fundamentos      Arquitectura     Teoría           Algoritmos
Matemáticos      y Bajo Nivel     y Formalismo     y Optimización
─────────────    ─────────────    ─────────────    ─────────────
MAT-101 (5)      SIS-201 (5)      TEO-301 (5)      ALG-401 (5)
MAT-102 (4)      SIS-202 (4)      TEO-302 (5)      ALG-402 (5)
MAT-103 (4)      LEN-201 (5)      MAT-301 (5)      MAT-401 (5)
MAT-104 (5)      ALG-201 (5)      MAT-302 (4)      ALG-403 (4)
SIS-101 (4)      SIS-203 (4)      TEO-303 (4)      TEO-401 (4)
INT-100 (3)      INT-200 (2)      INT-300 (2)      INT-400 (2)

CICLO V          CICLO VI         CICLO VII        CICLO VIII
Sistemas         IA y             Cripto, Seg.     Frontera
Complejos        Aprendizaje      y Distribuidos   y Síntesis
─────────────    ─────────────    ─────────────    ─────────────
SIS-501 (5)      IAP-601 (5)      SEG-701 (5)      ALG-801 (5)
LEN-501 (5)      IAP-602 (5)      SIS-701 (5)      IAP-801 (5)
SIS-502 (4)      IAP-603 (4)      SEG-702 (4)      INV-801 (4)
SIS-503 (5)      TEO-601 (5)      LEN-701 (5)      INV-802 (8)
LEN-502 (4)      MAT-601 (4)      SIS-702 (4)      Optativa (4)
INT-500 (2)      INT-600 (2)      INT-700 (2)
```

---

## 5. Grafo de prerrequisitos

Formato legible por agente: `CÓDIGO ← [prerrequisitos]`. `∅` = sin prerrequisito.

```
# CICLO I
MAT-101 ← ∅
MAT-102 ← ∅
MAT-103 ← ∅
MAT-104 ← ∅
SIS-101 ← ∅
INT-100 ← [MAT-101, SIS-101]           # concurrente

# CICLO II
SIS-201 ← [SIS-101]
SIS-202 ← [MAT-101]
LEN-201 ← [MAT-101, SIS-101]
ALG-201 ← [MAT-101, MAT-104, SIS-101]
SIS-203 ← [SIS-101]
INT-200 ← [SIS-201, SIS-202, LEN-201]  # concurrente

# CICLO III
TEO-301 ← [MAT-101]
TEO-302 ← [TEO-301]                    # concurrente permitido
MAT-301 ← [MAT-101, MAT-104]
MAT-302 ← [MAT-101]
TEO-303 ← [MAT-101]
INT-300 ← [TEO-301, TEO-302, MAT-301]  # concurrente

# CICLO IV
ALG-401 ← [ALG-201, MAT-104]
ALG-402 ← [ALG-401]                    # concurrente permitido
MAT-401 ← [MAT-102, MAT-103]
ALG-403 ← [ALG-201, SIS-201]
TEO-401 ← [MAT-104, MAT-302]
INT-400 ← [ALG-403, TEO-401, MAT-302]  # concurrente

# CICLO V
SIS-501 ← [SIS-201, SIS-203, ALG-403]
LEN-501 ← [LEN-201, TEO-301, SIS-201]
SIS-502 ← [SIS-201, MAT-104]
SIS-503 ← [SIS-203, ALG-201]
LEN-502 ← [LEN-201, TEO-303]
INT-500 ← [SIS-501, LEN-501, LEN-502]  # concurrente

# CICLO VI
IAP-601 ← [MAT-104, MAT-401, ALG-401]
IAP-602 ← [IAP-601]                    # concurrente permitido
IAP-603 ← [MAT-104, ALG-401]
TEO-601 ← [MAT-102, MAT-302, TEO-302]
MAT-601 ← [MAT-103, MAT-401]
INT-600 ← [IAP-602, MAT-601]           # concurrente

# CICLO VII
SEG-701 ← [MAT-302, MAT-104, TEO-302]
SIS-701 ← [SIS-501, SIS-502, ALG-403]
SEG-702 ← [SIS-201, SIS-501]
LEN-701 ← [LEN-201, LEN-502, TEO-303]
SIS-702 ← [ALG-403, SIS-201]
INT-700 ← [SEG-701, SIS-701, SIS-702]  # concurrente

# CICLO VIII
ALG-801 ← [ALG-402, TEO-302]
IAP-801 ← [IAP-602, SIS-702]
INV-801 ← [90 créditos aprobados]
INV-802 ← [INV-801, 160 créditos aprobados]
OPT-8xx ← [aprobación del comité + prerrequisitos del curso elegido]
```

**Validación del grafo.** Verificada la ausencia de ciclos y la satisfacibilidad de todo prerrequisito antes de su uso. Toda arista apunta de un ciclo anterior o igual al de la asignatura dependiente; las cuatro aristas intra-ciclo (`TEO-302 ← TEO-301`, `ALG-402 ← ALG-401`, `IAP-602 ← IAP-601`, más los INT-*) están marcadas como concurrentes y son las únicas del plan.

**Cadenas críticas** (ruta más larga; determinan el número mínimo de bloques secuenciales, no la duración en años):

```
SIS-101 → SIS-201 → SIS-501 → SIS-701                      (4 bloques)
MAT-101 → TEO-301 → TEO-302 → ALG-801                      (4 bloques)
MAT-101 → ALG-201 → ALG-401 → IAP-601 → IAP-602 → IAP-801  (6 bloques)
MAT-101 → LEN-201 → LEN-502 → LEN-701                      (4 bloques)
MAT-101 → ALG-201 → ALG-401 → IAP-601 → INV-801 → INV-802  (6 bloques)
```

**Consecuencia.** La cadena crítica es de 6 bloques. Ninguna ruta puede completar el programa en menos de 6 bloques secuenciales por razones de dependencia, con independencia de cuántas horas semanales tenga disponibles el estudiante. Si un bloque dura 16 semanas, el piso teórico es de 96 semanas ≈ 3 años; el piso **real** lo fija la carga total (§3.2) y está en §14.1.

---

## 6. Requisitos de graduación

| Requisito | Umbral |
|---|---|
| Créditos aprobados | 201 |
| Nota mínima aprobatoria | 14/20 (no hay redondeo al alza) |
| Pruebas de Dominio superadas | 39/39 — no son promediables ni recuperables por examen |
| Laboratorios integradores | 7/7 con defensa oral aprobada |
| Replicaciones completas de papers | 2 (INV-801) |
| Paper original evaluado por pares | 1 (INV-801) |
| Tesis | 40–80 páginas, contribución original, defensa ante comité de ≥3 doctores |
| Optativa de profundización | 1 asignatura de ≥4 créditos, aprobada por el comité |
| Bitácora metodológica | Serie completa de error de calibración por evaluación (§14.3) |

**Nota sobre el conteo de Pruebas de Dominio.** Son 39: una por asignatura no-integradora. Los 7 laboratorios integradores no tienen Prueba de Dominio, tienen artefacto con defensa oral. La optativa se rige por el instrumento de su curso fuente.

**Regla de no compensación.** Una Prueba de Dominio reprobada invalida la asignatura completa, sin importar el promedio de los demás instrumentos. El programa evalúa capacidad de producción, no acumulación de puntos.

**Titulaciones intermedias.** Como el programa completo excede 400 ECTS y las rutas realistas superan los 5 años, se definen dos hitos con valor propio, de modo que una interrupción no deje al estudiante sin nada acreditable:

| Hito | Requisito | Equivale a |
|---|---|---|
| **Certificado de Fundamentos** | Ciclos I–IV completos (24 unidades, 100 créditos, ≈5 500 h) | Base matemática y de sistemas comparable a un pregrado estándar completo |
| **Bachiller** | Ciclos I–VII + INV-801 (42 unidades, 189 créditos) | Habilitación para postular a posgrado en investigación |
| **Licenciado** | Todo lo anterior + INV-802 (tesis) + optativa | Título terminal |

---


---

## Malla curricular

Cada asignatura enlaza a su propia ficha (`coursepages/<código>/README.md`) con unidades semanales, bibliografía, Prueba de Dominio y protocolo de estudio. La columna **Carga** usa el formato `teoría–práctica–laboratorio / total semanal`.

### Ciclo I — Fundamentos Matemáticos

| Asignatura | Créditos | Carga | Prerrequisitos | ADN institucional |
|---|---|---|---|---|
| [MAT-101 — Matemáticas Discretas y Lógica Formal](coursepages/mat-101/README.md) **[NÚCLEO]** | 5 | 4–2–0 / 10 · **16 h/sem** | ∅ | MIT 6.1200[J] *(ex 6.042)* · UC Berkeley CS70 |
| [MAT-102 — Álgebra Lineal Computacional](coursepages/mat-102/README.md) **[NÚCLEO]** | 4 | 3–2–0 / 9 · **14 h/sem** | ∅ | MIT 18.06 (Strang) |
| [MAT-103 — Cálculo y Análisis Real para Computación](coursepages/mat-103/README.md) | 4 | 3–2–0 / 9 · **14 h/sem** | ∅ | MIT 18.100 |
| [MAT-104 — Probabilidad y Procesos Estocásticos](coursepages/mat-104/README.md) **[NÚCLEO]** | 5 | 4–2–0 / 10 · **16 h/sem** | ∅ | MIT 6.3700 *(ex 6.041)* · UC Berkeley EECS 126 · Harvard Stat 110 |
| [SIS-101 — Programación Científica y Sistemas](coursepages/sis-101/README.md) **[NÚCLEO]** | 4 | 2–0–4 / 8 · **14 h/sem** | ∅ | CMU 15-122 · MIT 6.1010 *(ex 6.009)* |
| [INT-100 — Laboratorio Integrador I](coursepages/int-100/README.md) | 3 | 0–0–4 / 6 · **10 h/sem** | MAT-101, SIS-101 (concurrentes) | — |

### Ciclo II — Arquitectura y Bajo Nivel

| Asignatura | Créditos | Carga | Prerrequisitos | ADN institucional |
|---|---|---|---|---|
| [SIS-201 — Organización y Arquitectura de Computadoras](coursepages/sis-201/README.md) **[NÚCLEO]** | 5 | 3–0–4 / 11 · **18 h/sem** | SIS-101 | CMU 15-213 / 18-213 — el curso de sistemas más influyente del planeta |
| [SIS-202 — Circuitos Digitales y Diseño Lógico](coursepages/sis-202/README.md) | 4 | 2–0–4 / 8 · **14 h/sem** | MAT-101 | MIT 6.1910 *(ex 6.004)* · CMU 18-240 |
| [LEN-201 — Lenguajes de Programación y Semántica](coursepages/len-201/README.md) **[NÚCLEO]** | 5 | 4–2–0 / 10 · **16 h/sem** | MAT-101, SIS-101 | CMU 15-150, 15-312 · MIT 6.820 |
| [ALG-201 — Estructuras de Datos Fundamentales](coursepages/alg-201/README.md) **[NÚCLEO]** | 5 | 3–2–2 / 9 · **16 h/sem** | MAT-101, MAT-104, SIS-101 | MIT 6.1210 *(ex 6.006)* · CMU 15-210 |
| [SIS-203 — Arquitectura de Memoria y Almacenamiento](coursepages/sis-203/README.md) | 4 | 3–0–2 / 9 · **14 h/sem** | SIS-101 | CMU 15-445 (fundamentos de almacenamiento) · Stanford CS145 |
| [INT-200 — Laboratorio Integrador II](coursepages/int-200/README.md) | 2 | 0–0–3 / 5 · **8 h/sem** | SIS-201, SIS-202, LEN-201 (concurrentes) | — |

### Ciclo III — Teoría y Formalismo

| Asignatura | Créditos | Carga | Prerrequisitos | ADN institucional |
|---|---|---|---|---|
| [TEO-301 — Autómatas, Lenguajes y Computabilidad](coursepages/teo-301/README.md) **[NÚCLEO]** | 5 | 4–2–0 / 11 · **17 h/sem** | MAT-101 | MIT 18.404[J] / 6.5400[J] — el curso de Sipser |
| [TEO-302 — Teoría de la Complejidad Computacional](coursepages/teo-302/README.md) **[NÚCLEO]** | 5 | 4–2–0 / 12 · **18 h/sem** | TEO-301 (concurrente permitido) | UC Berkeley CS172 · MIT 6.1400[J] *(ex 6.045)* · MIT 6.5400 |
| [MAT-301 — Teoría de Grafos y Combinatoria Avanzada](coursepages/mat-301/README.md) | 5 | 4–2–0 / 11 · **17 h/sem** | MAT-101, MAT-104 | MIT 18.217 · CMU 21-701 |
| [MAT-302 — Álgebra Abstracta para Computación](coursepages/mat-302/README.md) | 4 | 3–2–0 / 9 · **14 h/sem** | MAT-101 | MIT 18.703 · UC Berkeley Math 113 |
| [TEO-303 — Lógica Matemática y Teoría de Modelos](coursepages/teo-303/README.md) | 4 | 3–2–0 / 9 · **14 h/sem** | MAT-101 | UC Berkeley Math 125A · MIT 18.510 |
| [INT-300 — Laboratorio Integrador III](coursepages/int-300/README.md) | 2 | 0–0–3 / 5 · **8 h/sem** | TEO-301, TEO-302, MAT-301 (concurrentes) | — |

### Ciclo IV — Algoritmos y Optimización

| Asignatura | Créditos | Carga | Prerrequisitos | ADN institucional |
|---|---|---|---|---|
| [ALG-401 — Diseño y Análisis de Algoritmos](coursepages/alg-401/README.md) **[NÚCLEO]** | 5 | 4–2–0 / 11 · **17 h/sem** | ALG-201, MAT-104 | MIT 6.1220[J] / 18.410[J] *(ex 6.046)* |
| [ALG-402 — Algoritmos Avanzados y Geometría Computacional](coursepages/alg-402/README.md) | 5 | 4–2–0 / 12 · **18 h/sem** | ALG-401 (concurrente permitido) | MIT 6.5210[J] / 18.415[J] *(ex 6.854, Karger)* · Stanford CS261 |
| [MAT-401 — Álgebra Lineal Numérica y Optimización](coursepages/mat-401/README.md) **[NÚCLEO]** | 5 | 4–2–0 / 11 · **17 h/sem** | MAT-102, MAT-103 | Stanford EE364A/B (Boyd) · MIT 18.085 |
| [ALG-403 — Computación Paralela y Distribuida](coursepages/alg-403/README.md) | 4 | 2–0–4 / 8 · **14 h/sem** | ALG-201, SIS-201 | CMU 15-210 · Stanford CS149 · MIT 6.106 *(ex 6.172)* |
| [TEO-401 — Teoría de la Información y Códigos](coursepages/teo-401/README.md) | 4 | 3–2–0 / 9 · **14 h/sem** | MAT-104, MAT-302 | MIT 6.441[J] · Stanford EE376A |
| [INT-400 — Laboratorio Integrador IV](coursepages/int-400/README.md) | 2 | 0–0–3 / 5 · **8 h/sem** | ALG-403, TEO-401, MAT-302 (concurrentes) | — |

### Ciclo V — Sistemas Complejos

| Asignatura | Créditos | Carga | Prerrequisitos | ADN institucional |
|---|---|---|---|---|
| [SIS-501 — Sistemas Operativos Internos](coursepages/sis-501/README.md) **[NÚCLEO]** | 5 | 3–0–4 / 12 · **19 h/sem** | SIS-201, SIS-203, ALG-403 | CMU 15-410 · MIT 6.1810 *(ex 6.S081 / 6.828)* |
| [LEN-501 — Diseño de Compiladores](coursepages/len-501/README.md) **[NÚCLEO]** | 5 | 3–0–4 / 11 · **18 h/sem** | LEN-201, TEO-301, SIS-201 | Stanford CS143 · CMU 15-411 |
| [SIS-502 — Redes de Computadoras: Protocolos y Arquitectura](coursepages/sis-502/README.md) | 4 | 2–0–4 / 8 · **14 h/sem** | SIS-201, MAT-104 | Stanford CS144 · MIT 6.829 |
| [SIS-503 — Bases de Datos: Motores e Internals](coursepages/sis-503/README.md) **[NÚCLEO]** | 5 | 3–0–4 / 11 · **18 h/sem** | SIS-203, ALG-201 | CMU 15-445 / 645 (Andrew Pavlo) |
| [LEN-502 — Verificación Formal y Métodos Formales](coursepages/len-502/README.md) | 4 | 3–2–0 / 9 · **14 h/sem** | LEN-201, TEO-303 | CMU 15-414 · MIT 6.820 |
| [INT-500 — Laboratorio Integrador V](coursepages/int-500/README.md) | 2 | 0–0–3 / 5 · **8 h/sem** | SIS-501, LEN-501, LEN-502 (concurrentes) | — |

### Ciclo VI — IA y Aprendizaje

| Asignatura | Créditos | Carga | Prerrequisitos | ADN institucional |
|---|---|---|---|---|
| [IAP-601 — Fundamentos Matemáticos del Aprendizaje Automático](coursepages/iap-601/README.md) **[NÚCLEO]** | 5 | 4–2–0 / 11 · **17 h/sem** | MAT-104, MAT-401, ALG-401 | Stanford CS229 · UC Berkeley CS189 — vertiente teórica |
| [IAP-602 — Redes Neuronales Profundas: Teoría y Arquitecturas](coursepages/iap-602/README.md) **[NÚCLEO]** | 5 | 3–0–4 / 11 · **18 h/sem** | IAP-601 (concurrente permitido) | Stanford CS231N y CS224N · MIT 6.S191 |
| [IAP-603 — Inteligencia Artificial: Búsqueda, Planificación y Razonamiento](coursepages/iap-603/README.md) | 4 | 3–2–0 / 9 · **14 h/sem** | MAT-104, ALG-401 | UC Berkeley CS188 · Stanford CS221 — vertiente teórica |
| [TEO-601 — Computación Cuántica: Teoría y Algoritmos](coursepages/teo-601/README.md) | 5 | 4–2–0 / 11 · **17 h/sem** | MAT-102, MAT-302, TEO-302 | MIT 8.370[J] / 18.435[J] · UC Berkeley CS294 |
| [MAT-601 — Geometría Diferencial y Álgebra Tensorial para Aprendizaje](coursepages/mat-601/README.md) | 4 | 3–2–0 / 9 · **14 h/sem** | MAT-103, MAT-401 | Stanford CS468 · MIT 18.950 |
| [INT-600 — Laboratorio Integrador VI](coursepages/int-600/README.md) | 2 | 0–0–3 / 5 · **8 h/sem** | IAP-602, MAT-601 (concurrentes) | — |

### Ciclo VII — Criptografía, Seguridad y Distribuidos

| Asignatura | Créditos | Carga | Prerrequisitos | ADN institucional |
|---|---|---|---|---|
| [SEG-701 — Criptografía: Fundamentos Matemáticos y Protocolos](coursepages/seg-701/README.md) **[NÚCLEO]** | 5 | 4–2–0 / 12 · **18 h/sem** | MAT-302, MAT-104, TEO-302 | UC Berkeley CS276 · MIT 6.5620 / 18.425 *(ex 6.875)* · Stanford CS255 |
| [SIS-701 — Sistemas Distribuidos: Teoría y Construcción](coursepages/sis-701/README.md) **[NÚCLEO]** | 5 | 3–0–4 / 11 · **18 h/sem** | SIS-501, SIS-502, ALG-403 | MIT 6.5840 *(ex 6.824)* · CMU 15-440 |
| [SEG-702 — Seguridad de Sistemas y Ataques a Bajo Nivel](coursepages/seg-702/README.md) | 4 | 2–0–4 / 8 · **14 h/sem** | SIS-201, SIS-501 | CMU 15-330 · UC Berkeley CS161 · Stanford CS155 |
| [LEN-701 — Tipos Dependientes y Verificación Mecanizada](coursepages/len-701/README.md) | 5 | 3–2–2 / 10 · **17 h/sem** | LEN-201, LEN-502, TEO-303 | CMU 15-317 y 15-819 · MIT 6.826 |
| [SIS-702 — Computación de Alto Rendimiento y Arquitecturas Especializadas](coursepages/sis-702/README.md) | 4 | 2–0–4 / 8 · **14 h/sem** | ALG-403, SIS-201 | Stanford CS315A · MIT 6.106 *(ex 6.172)* · CMU 15-418/618 |
| [INT-700 — Laboratorio Integrador VII](coursepages/int-700/README.md) | 2 | 0–0–3 / 5 · **8 h/sem** | SEG-701, SIS-701, SIS-702 (concurrentes) | — |

### Ciclo VIII — Frontera y Síntesis

| Asignatura | Créditos | Carga | Prerrequisitos | ADN institucional |
|---|---|---|---|---|
| [ALG-801 — Complejidad Fina y Algoritmos de Frontera](coursepages/alg-801/README.md) | 5 | 4–2–0 / 12 · **18 h/sem** | ALG-402, TEO-302 | MIT 6.890 *(R. Williams & V. Vassilevska Williams)* · UC Berkeley CS294 |
| [IAP-801 — Modelos de Lenguaje: Teoría y Escalamiento](coursepages/iap-801/README.md) | 5 | 3–0–4 / 11 · **18 h/sem** | IAP-602, SIS-702 | **Stanford CS336 — *Language Modeling from Scratch* (Liang & Hashimoto, edición Spring 2026)** · MIT 6.S965 |
| [INV-801 — Seminario de Investigación: Metodología y Literatura Primaria](coursepages/inv-801/README.md) | 4 | 2–2–0 / 12 · **16 h/sem** | 90 créditos aprobados | Seminario doctoral de MIT, CMU, Stanford y Berkeley, adaptado a pregrado |
| [INV-802 — Proyecto de Investigación de Síntesis (Tesis)](coursepages/inv-802/README.md) | 8 | 0–0–6 / 20 · **26 h/sem** | INV-801, 160 créditos aprobados | MIT UROP · CMU Senior Thesis · Stanford Honors Program |
| [OPT-001 — Optativa de Profundización](coursepages/opt-001/README.md) | 4 | variable · **≈14 h/sem** | según la asignatura elegida | — |

---

## Documentos del repositorio

| Archivo | Contenido |
|---|---|
| [`METHODOLOGY.md`](METHODOLOGY.md) | Sistema de evaluación, mecanismos de aprendizaje, sustrato neurobiológico, sueño, carga cognitiva, repaso espaciado, régimen semanal, rutas de titulación, uso de LLMs, prácticas desacreditadas, protocolo de reingreso (§7–§18 del documento original) |
| [`RESOURCES.md`](RESOURCES.md) | Cursos fuente por institución, libros de acceso abierto, herramientas, plataformas de práctica, evaluación externa, venues de investigación (§19–§24) |
| [`APPENDIX.md`](APPENDIX.md) | Índice de asignaturas, presupuesto de horas, matriz asignatura×competencia, distribución de dificultad, trazabilidad de Pruebas de Dominio, ruta de nivelación, instrucciones de uso para agente (§25–§31) |
| [`VERIFICATION.md`](VERIFICATION.md) | Estado de verificación de fuentes primarias |
| [`REFERENCES.md`](REFERENCES.md) | Bibliografía completa por capa |
| [`EXCLUSIONS.md`](EXCLUSIONS.md) | Qué queda fuera del programa y por qué |
| [`CHANGELOG.md`](CHANGELOG.md) | Registro de cambios 2026.1 → 2026.2 → 2026.3 |
| [`FAQ.md`](FAQ.md) | Preguntas frecuentes |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Cómo evoluciona este documento |

## Cómo mostrar tu progreso

Haz fork de este repo y marca ✅ junto a cada asignatura en las tablas de arriba conforme la completes. Sirve como kanban board de tu propio avance.

## Licencia

MIT — ver [`LICENSE`](LICENSE).
