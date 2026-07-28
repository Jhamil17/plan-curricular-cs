### SIS-501 — Sistemas Operativos Internos — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 12 · **19 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-201, SIS-203, ALG-403 |
| **ADN institucional** | CMU 15-410 · MIT 6.1810 *(ex 6.S081 / 6.828)* |

**Competencia terminal.** Construye un núcleo funcional con planificación, memoria virtual y sistema de archivos, y razona sobre sus propiedades de seguridad y ausencia de bloqueo.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Procesos y arranque | Arranque y modo protegido · PCB · Cambio de contexto · ABI de llamadas al sistema · Trampas, interrupciones y excepciones |
| 2 | 4–6 | Planificación | FCFS, SJF, Round Robin · CFS/EEVDF de Linux · Prioridades e inversión de prioridad · Métricas: utilización, throughput, turnaround, equidad · Planificación en multiprocesador |
| 3 | 7–9 | Concurrencia en el núcleo | Semáforos, mutex, monitores, variables de condición · Condiciones de Coffman · Detección por grafo de recursos · Prevención · Algoritmo del banquero · Bloqueo en vivo |
| 4 | 10–12 | Memoria virtual | Paginación y tablas multinivel · Manejo de fallos de página · Demand paging y swap · mmap · Copy-on-write · TLB shootdown en SMP |
| 5 | 13–15 | Persistencia y aislamiento | VFS · Inodos · Journaling ext4 · Crash consistency · io_uring y epoll · Drivers: interrupciones y DMA · Anillos de privilegio x86 · seccomp-bpf, namespaces, cgroups |

**Laboratorios.** L1 llamadas al sistema · L2 planificador · L3 paginación · L4 copy-on-write fork · L5 hilos a nivel de usuario · L6 sistema de archivos · L7 red o mmap.

**Prueba de Dominio.** Núcleo minimalista completo (base xv6 o PintOS) con: planificador de hilos reales, memoria virtual con paginación y COW, y sistema de archivos con journaling. Sometido a inyección de fallos por corte de energía simulado en punto arbitrario, con análisis formal de ausencia de deadlock en la jerarquía de bloqueos.

**Bibliografía.**
- **Base:** *Operating Systems: Three Easy Pieces* — Arpaci-Dusseau & Arpaci-Dusseau (gratuito) + código fuente comentado de xv6
- **Complementaria:** *Lions' Commentary on UNIX 6th Edition* · *Understanding the Linux Kernel* — Bovet & Cesati · *Operating Systems: Principles and Practice* — Anderson & Dahlin
- **Papers:** *"The UNIX Time-Sharing System"* — Ritchie & Thompson (CACM 1974)

**Recursos.** pdos.csail.mit.edu/6.828 (xv6 + labs completos) · pages.cs.wisc.edu/~remzi/OSTEP · QEMU + GDB para depuración de núcleo · CMU 15-410 (PintOS).

**Protocolo de estudio.** La asignatura de mayor carga cognitiva del programa. Regla estricta: **un subsistema por semana**, con la especificación escrita antes del código. Nunca depurar dos subsistemas simultáneamente — en un núcleo, dos bugs simultáneos producen síntomas que no corresponden a ninguno de los dos.

---

