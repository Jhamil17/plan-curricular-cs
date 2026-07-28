### IAP-801 — Modelos de Lenguaje: Teoría y Escalamiento

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | IAP-602, SIS-702 |
| **ADN institucional** | **Stanford CS336 — *Language Modeling from Scratch* (Liang & Hashimoto, edición Spring 2026)** · MIT 6.S965 |

**Competencia terminal.** Construye la pila completa de un modelo de lenguaje y razona cuantitativamente sobre el compromiso entre cómputo, datos y parámetros.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Tokenización y contabilidad de recursos | BPE y variantes byte-level · Patologías de tokenización · Contabilidad de FLOPs, memoria y ancho de banda · Presupuesto de cómputo del entrenamiento |
| 2 | 4–6 | Arquitectura y sistemas | Transformer decoder-only en detalle · Normalización y ubicación de la norma · RoPE · Atención agrupada (GQA/MQA) · Kernels y FlashAttention · **Mixture-of-experts: routing, balanceo de carga, capacidad** · Paralelismo de datos, tensor, pipeline y secuencia |
| 3 | 7–9 | Leyes de escalamiento | Kaplan et al.: relaciones potenciales entre pérdida, parámetros, datos y cómputo · Chinchilla: punto óptimo de cómputo · Derivación desde primeros principios estadísticos · **Crítica de las "habilidades emergentes": dependencia de la métrica (Schaeffer et al.)** |
| 4 | 10–12 | Datos y alineamiento | Curación y deduplicación · Contaminación de benchmarks · RLHF con PPO: KL como regularización, reward hacking · DPO y métodos sin modelo de recompensa · RLAIF / Constitutional AI · **RL con recompensa verificable y cómputo en tiempo de inferencia** |
| 5 | 13–15 | Inferencia e interpretabilidad | KV-cache · Decodificación especulativa · Cuantización: GPTQ, AWQ · Batching continuo y PagedAttention · **Interpretabilidad mecanística: superposición, monosemanticidad, sparse autoencoders, análisis de circuitos** · Memorización y capacidad · Jailbreaking y prompt injection como problema formal |

**Prueba de Dominio.** Derivación analítica de las leyes de escalamiento desde primeros principios estadísticos + implementación de un Transformer decoder-only con KV-cache y decodificación especulativa, con predicción teórica de la mejora de throughput contrastada contra la medición real y la discrepancia explicada desde el modelo roofline de SIS-702.

**Bibliografía.**
- **Base:** Materiales públicos de Stanford CS336 (lecturas, assignments y video de la edición vigente)
- **Complementaria:** *Understanding Deep Learning* — Prince (base arquitectónica) · *Speech and Language Processing* (3ª ed. en borrador) — Jurafsky & Martin (gratuito)
- **Papers:** *"Attention Is All You Need"* — Vaswani et al. (2017) · *"Scaling Laws for Neural Language Models"* — Kaplan et al. (2020) · *"Training Compute-Optimal Large Language Models"* — Hoffmann et al. (2022) · *"Are Emergent Abilities of Large Language Models a Mirage?"* — Schaeffer, Miranda & Koyejo (NeurIPS 2023) · *"Toy Models of Superposition"* — Elhage et al. (Anthropic, 2022) · *"Direct Preference Optimization"* — Rafailov et al. (NeurIPS 2023)

**Recursos.** cs336.stanford.edu (**verificar edición vigente**) · web.stanford.edu/~jurafsky/slp3 · transformer-circuits.pub · Papers with Code y ECCC/arXiv para seguimiento.

**Protocolo de estudio.** Asignatura de vida media corta. Los papers se leen con el protocolo de tres pasadas (Keshav) y toda afirmación empírica se marca explícitamente como **replicada** o **no replicada**. Solo lo estructural entra al mazo FSRS —arquitectura, contabilidad de recursos, derivaciones—; lo coyuntural (números de un modelo concreto, resultados de un benchmark) no entra nunca.

---

