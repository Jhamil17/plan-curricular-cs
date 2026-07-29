### SIS-201 — Organización y Arquitectura de Computadoras — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-101 |
| **ADN institucional** | CMU 15-213 / 18-213 — el curso de sistemas más influyente del planeta |

**Competencia terminal.** Predice el rendimiento de un programa desde su patrón de acceso a memoria y desde el comportamiento del pipeline, y explota las consecuencias de una representación mal validada.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Representación de la información | Complemento a dos · Desbordamiento · IEEE 754: precisión simple y doble, NaN, Inf, subnormales · Consecuencias de la no asociatividad del punto flotante |
| 2 | 4–6 | ISA y ensamblador x86-64 | Registros · Modos de direccionamiento · ABI System V · Aritmética, lógica, saltos · Stack frames · Convención de llamadas |
| 3 | 7–9 | Ejecución y pipeline | Etapas IF, ID, EX, MEM, WB · Hazards de datos, estructurales y de control · Forwarding · Predicción de saltos: BTB, tournament predictors · Ejecución especulativa |
| 4 | 10–12 | Jerarquía de memoria | SRAM, DRAM, disco · Localidad espacial y temporal · Caché directa, asociativa por conjuntos, totalmente asociativa · Políticas LRU, LFU, RRIP · NUMA |
| 5 | 13–15 | Optimización guiada por arquitectura | Cache-oblivious algorithms · Blocking y tiling · Prefetching · Medición con `perf` · Memory mountain |

**Laboratorios (los labs canónicos de CMU).** L1 *data lab* · L2 *bomb lab* (desensamblado) · L3 *attack lab* (buffer overflow, ROP) · L4 *cache lab* (simulador + optimización de transposición) · L5 *performance lab*.

**Prueba de Dominio.** *Attack lab* completo (explotación de stack y return-oriented programming) + *cache lab* (simulador de caché e optimización de multiplicación de matrices con maximización medida del hit rate y justificación desde el modelo de jerarquía).

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del simulador y de la multiplicación optimizada, con el escalamiento declarado respecto a la dimensión de la matriz y al tamaño de la traza. El número que decide algo es el **tamaño de bloque**: se deriva del tamaño y la asociatividad de la caché medidos, no se busca por prueba y error, y la distancia entre el bloque derivado y el óptimo empírico es el resultado — si difieren, el modelo de jerarquía está incompleto y hay que decir en qué.

**Bibliografía.**
- **Base:** *Computer Systems: A Programmer's Perspective* (3ª ed., 2016) — Bryant & O'Hallaron · **CSAPP; edición vigente**
- **Complementaria:** *Computer Architecture: A Quantitative Approach* (6ª ed.) — Hennessy & Patterson
- **Papers:** *"What Every Programmer Should Know About Memory"* — Drepper (2007)

**Recursos.** csapp.cs.cmu.edu (labs públicos con autograder local) · Compiler Explorer · `perf`, `valgrind --tool=cachegrind`, Intel VTune.

**Protocolo de estudio.** Asignatura con la mayor densidad de tarjetas de traza: estado de registros y de caché tras N instrucciones. Los labs se atacan sin escribir código el primer día — solo lectura de desensamblado y predicción en papel.

---

