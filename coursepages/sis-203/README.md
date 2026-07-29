### SIS-203 — Arquitectura de Memoria y Almacenamiento

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–0–2 / 9 · **14 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-101 |
| **ADN institucional** | CMU 15-445 (fundamentos de almacenamiento) · Stanford CS145 |

**Competencia terminal.** Diseña la capa de almacenamiento de un sistema con conocimiento explícito del costo real de cada nivel de la jerarquía.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Memoria virtual | Paginación · TLB · Tablas de páginas multinivel (x86-64: PML4) · Segmentación vs paginación · Páginas grandes |
| 2 | 4–6 | Políticas de reemplazo | OPT (Bélády) como cota · LRU, LRU-K, Clock, ARC · Working set theory · Thrashing |
| 3 | 7–9 | Dispositivos | HDD: seek time, latencia rotacional · SSD: NAND, FTL, wear leveling, write amplification · NVMe · Persistent memory |
| 4 | 10–12 | Redundancia y sistemas de archivos | RAID 0/1/5/6 con análisis de MTTF · FAT, ext4, XFS · Journaling · Crash consistency · Log-structured file systems |
| 5 | 13–15 | Buffer pool | Gestión de páginas en memoria · Pinning y latching · Páginas sucias · Políticas de escritura · Prefetching de secuencias |

**Prueba de Dominio.** Buffer pool manager con política LRU-K y extendible hashing para un motor de base de datos minimalista (estilo BusTub, CMU DB Group), evaluado contra trazas reales de acceso y contra la cota OPT.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del buffer pool y se declara su escalamiento respecto al tamaño de la traza y al número de marcos, contrastado contra la complejidad derivada.

**Bibliografía.**
- **Base:** *Operating Systems: Three Easy Pieces* — Arpaci-Dusseau & Arpaci-Dusseau (OSTEP, gratuito), partes de virtualización y persistencia
- **Complementaria:** *Database Internals* — Petrov (capítulos de almacenamiento)
- **Papers:** *"The LRU-K Page Replacement Algorithm for Database Disk Buffering"* — O'Neil, O'Neil & Weikum (SIGMOD 1993) · *"ARC: A Self-Tuning, Low Overhead Replacement Cache"* — Megiddo & Modha (FAST 2003)

**Recursos.** pages.cs.wisc.edu/~remzi/OSTEP (libro completo gratuito) · 15445.courses.cs.cmu.edu · fio y blktrace para caracterizar dispositivos reales.

**Protocolo de estudio.** Cada política de reemplazo se evalúa contra una traza real y contra OPT. La métrica es la distancia al óptimo, no el hit rate absoluto: un hit rate alto sobre una traza fácil no dice nada.

---

