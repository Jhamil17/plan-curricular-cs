### SIS-701 — Sistemas Distribuidos: Teoría y Construcción — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-501, SIS-502, ALG-403 |
| **ADN institucional** | MIT 6.5840 *(ex 6.824)* · CMU 15-440 |

**Competencia terminal.** Implementa un protocolo de consenso correcto bajo fallas y demuestra qué garantías son imposibles en el modelo dado.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelos e imposibilidades | Modelos de sincronía: síncrono, asíncrono, parcialmente síncrono · Modelos de falla: crash-stop, omisión, bizantino · **Teorema FLP con demostración completa** · Teorema CAP con demostración · Detectores de fallos |
| 2 | 4–6 | Tiempo y causalidad | Relojes de Lamport · Relojes vectoriales (Mattern, Fidge) · Relación happened-before · Cortes consistentes · Snapshot de Chandy-Lamport |
| 3 | 7–9 | Modelos de consistencia | Linearizabilidad · Serializabilidad · Consistencia secuencial · Consistencia causal · Consistencia eventual · Jerarquía completa y sus costos · CRDTs |
| 4 | 10–12 | Consenso | Paxos: Single-Decree y Multi-Paxos, safety y liveness · Raft: elección de líder, replicación de log, compactación, cambio de configuración · Replicación de máquinas de estado · Viewstamped Replication · BFT: PBFT con análisis de f ≤ ⌊(n−1)/3⌋ |
| 5 | 13–15 | Sistemas reales | DHT: Chord con análisis de O(log n) saltos · Sistemas de archivos distribuidos: GFS, Ceph · Transacciones distribuidas: 2PC, 3PC · Spanner y TrueTime · Protocolos gossip y modelos epidémicos |

**Laboratorios.** L1 MapReduce · L2 Raft: elección de líder · L3 Raft: replicación de log · L4 Raft: persistencia y compactación · L5 servicio clave-valor tolerante a fallos · L6 fragmentación (sharding).

**Prueba de Dominio.** Demostración completa del Teorema FLP + implementación funcional del protocolo Raft con prueba de que mantiene la propiedad de log matching bajo fallas de crash arbitrarias. Evaluado bajo particiones de red, reordenamiento y pérdida de mensajes inyectados de forma determinista y reproducible.

**Instrumentación obligatoria (§15.7).** La implementación debe exponer latencia de commit como distribución (p50 y p99), tasa de error —peticiones rechazadas, elecciones fallidas, pérdida de liderazgo— y saturación del recurso que primero se agota: ventana de replicación pendiente, retraso del log del seguidor más lento, tamaño del log antes de compactación. **Criterio-compuerta:** un Raft funcionalmente correcto que no expone las tres señales tiene la Prueba de Dominio no superada (§6).

**Contabilidad de costo (§15.8).** Se acota cómputo, memoria y mensajes por operación de consenso, y se declara su escalamiento respecto al número de nodos y al tamaño del log, contrastado contra la complejidad derivada.

**Bibliografía.**
- **Base:** *Designing Data-Intensive Applications* (**2ª ed., marzo 2026**) — Kleppmann & Riccomini
- **Complementaria:** *Distributed Systems* (4ª ed.) — van Steen & Tanenbaum (gratuito) · *Introduction to Reliable and Secure Distributed Programming* — Cachin, Guerraoui & Rodrigues
- **Papers:** *"Impossibility of Distributed Consensus with One Faulty Process"* — Fischer, Lynch & Paterson (JACM 1985) · *"In Search of an Understandable Consensus Algorithm"* — Ongaro & Ousterhout (USENIX ATC 2014) · *"Paxos Made Simple"* — Lamport (2001) · *"Time, Clocks, and the Ordering of Events"* — Lamport (CACM 1978) · *"Spanner: Google's Globally-Distributed Database"* — Corbett et al. (OSDI 2012)

**Recursos.** pdos.csail.mit.edu/6.824 (labs completos en Go + video) · distributed-systems.net (van Steen gratuito) · raft.github.io (visualización) · TLA+ para especificar el protocolo antes de implementarlo · Jepsen como referencia de metodología de testing.

**Protocolo de estudio.** Toda implementación se somete a particiones y reordenamiento de mensajes inyectados de forma determinista. Un Raft que pasa el camino feliz no está implementado: está esbozado. Especificar en TLA+ antes de codificar reduce el tiempo total, no lo aumenta.

---

