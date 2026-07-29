### SIS-702 — Computación de Alto Rendimiento y Arquitecturas Especializadas

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | ALG-403, SIS-201 |
| **ADN institucional** | Stanford CS315A · MIT 6.106 *(ex 6.172)* · CMU 15-418/618 |

**Competencia terminal.** Explica cada optimización de rendimiento desde un modelo cuantitativo y alcanza una fracción justificada del límite teórico del hardware.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelos de rendimiento | Roofline: intensidad aritmética, límite por memoria vs por cómputo · Amdahl refinado con overhead de comunicación · Medición correcta: varianza, warm-up, efectos de frecuencia |
| 2 | 4–6 | Optimización en CPU | SIMD: AVX-512, vectorización automática y manual, operaciones de carril · Loop tiling y blocking multinivel · Análisis del working set · Prefetching de hardware y software · Row buffer locality en DRAM |
| 3 | 7–9 | Arquitectura GPU | Modelo SIMT · Warps y divergencia · Ocupancia · Jerarquía de memoria: global, shared, L1/L2 · Memory coalescing · Bank conflicts |
| 4 | 10–12 | Programación CUDA | Modelo de ejecución y de memoria · Optimización de kernels · Streams y solapamiento · Tensor cores · Cuantización: INT8, FP16, BF16, FP8 · Perfilado con Nsight |
| 5 | 13–15 | Escala distribuida | Redes de interconexión: bisection bandwidth, fat-tree, torus, routing · MPI: punto a punto y colectivos (barrier, broadcast, reduce, all-reduce) · Modelos SPMD y BSP · Paralelismo de datos, de tensor y de pipeline |

**Prueba de Dominio.** Multiplicación de matrices densa (GEMM) en CUDA que alcance ≥90% de la eficiencia del roofline teórico de la GPU disponible, mediante uso de memoria compartida, vectorización y ocultamiento de latencia. Cada paso de optimización documentado con medición antes/después y explicación causal desde el modelo.

**Contabilidad de costo (§15.8).** Se acota cómputo (FLOPs contados y medidos), memoria y **precio por GPU-hora** del proveedor citado como constante declarada, y se declara el escalamiento del costo respecto a la dimensión de la matriz, contrastado contra el techo del roofline.

**Bibliografía.**
- **Base:** *Programming Massively Parallel Processors* (4ª ed.) — Kirk, Hwu & El Hajj
- **Complementaria:** *Computer Architecture: A Quantitative Approach* (6ª ed.) — Hennessy & Patterson · *Performance Analysis and Tuning on Modern CPUs* — Bakhvalov (gratuito)
- **Papers:** *"Roofline: An Insightful Visual Performance Model"* — Williams, Waterman & Patterson (CACM 2009)

**Recursos.** CMU 15-418 (video completo) · MIT 6.106 · Documentación del vendor de la GPU disponible (**verificar generación y guía de tuning vigente**) · Nsight Compute, `perf`, likwid · CUTLASS como referencia de GEMM optimizado.

**Protocolo de estudio.** Ninguna optimización se acepta sin medición antes/después **y** sin explicación causal desde el modelo roofline. Optimizar sin modelo es superstición: produce mejoras que no se transfieren y regresiones que no se explican.

---

