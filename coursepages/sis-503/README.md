### SIS-503 — Bases de Datos: Motores e Internals — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-203, ALG-201 |
| **ADN institucional** | CMU 15-445 / 645 (Andrew Pavlo) |

**Competencia terminal.** Construye un motor relacional transaccional con recuperación ante fallos y control de concurrencia demostrablemente serializable.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelo y almacenamiento | Álgebra relacional · Cálculo relacional de tuplas y de dominio · Formato de página y de tupla · Almacenamiento por filas vs por columnas · Compresión |
| 2 | 4–6 | Índices | B+-Trees: estructura, división, fusión, concurrencia por latch crabbing · Hash extensible y lineal · LSM-trees y estrategias de compactación · Índices de cobertura |
| 3 | 7–9 | Ejecución de consultas | Modelo Volcano de iteradores · Ejecución vectorizada · Joins: Nested Loop, Block Nested Loop, Sort-Merge con análisis exacto de I/O, Hash Join (Grace, Hybrid) · Agregación y ordenamiento externos |
| 4 | 10–12 | Optimización | Estimación de cardinalidad · Histogramas y sketches · Estadísticas · Optimización basada en costos (Selinger, System R) · Reordenamiento de joins · Materialización tardía |
| 5 | 13–15 | Transacciones y recuperación | ACID · 2PL y 2PL estricto · Detección y prevención de deadlock · Niveles de aislamiento · Snapshot isolation y sus anomalías (write skew) · MVCC · WAL · ARIES: Analysis, Redo, Undo |

**Prueba de Dominio.** Motor de base de datos completo desde cero (referencia: BusTub de CMU) con buffer pool manager, tabla hash extensible, índice B+Tree concurrente, motor de ejecución con join y agregación, control de concurrencia por 2PL y recuperación ARIES. Validado con inyección de crash en punto arbitrario y verificación de serializabilidad sobre historias generadas.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del motor y se declara su escalamiento respecto al tamaño de la relación y al número de transacciones concurrentes, contrastado contra la complejidad derivada.

**Bibliografía.**
- **Base:** *Database Internals* — Alex Petrov
- **Complementaria:** *Database System Concepts* (7ª ed.) — Silberschatz, Korth & Sudarshan · *Readings in Database Systems* ("Red Book", 5ª ed., gratuito) · *Transaction Processing* — Gray & Reuter
- **Papers:** *"Architecture of a Database System"* — Hellerstein, Stonebraker & Hamilton (2007) · *"ARIES: A Transaction Recovery Method..."* — Mohan et al. (TODS 1992) · *"Access Path Selection in a Relational DBMS"* — Selinger et al. (SIGMOD 1979)

**Recursos.** 15445.courses.cs.cmu.edu (curso completo en video + proyectos BusTub con autograder) · redbook.io · PostgreSQL como referencia de implementación madura.

**Protocolo de estudio.** Ningún componente se considera terminado antes de someterlo a inyección de fallos en punto arbitrario. La recuperación es la especificación, no una función añadida al final.

---

