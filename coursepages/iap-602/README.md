### IAP-602 — Redes Neuronales Profundas: Teoría y Arquitecturas — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 3–0–4 / 11 · **18 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | IAP-601 (concurrente permitido) |
| **ADN institucional** | Stanford CS231N y CS224N · MIT 6.S191 |

**Competencia terminal.** Deriva analíticamente el gradiente de cualquier capa y construye arquitecturas modernas sin frameworks de alto nivel.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Diferenciación y optimización | Diferenciación automática: modo forward vs reverse, grafos de cómputo, tape-based AD · Derivación exacta de gradientes para capas densas · Gradient checking numérico · SGD, Adam/AdamW con análisis de convergencia · Schedules |
| 2 | 4–6 | Estabilidad del entrenamiento | Vanishing y exploding gradients: análisis espectral del Jacobiano · Inicialización (Xavier, He) · Batch norm, layer norm, RMSNorm · Conexiones residuales y su efecto sobre el paisaje de pérdida · Teorema de aproximación universal (Cybenko, Hornik) |
| 3 | 7–9 | Arquitecturas convolucionales y recurrentes | Convolución vs correlación cruzada · Campo receptivo · Conteo de parámetros · AlexNet → VGG → ResNet → EfficientNet · RNN y BPTT · LSTM: compuertas y flujo de gradiente · GRU |
| 4 | 10–12 | Atención y Transformers | Scaled dot-product attention con análisis O(n²d) · Multi-head · Codificación posicional: absoluta, RoPE, ALiBi · Arquitectura completa del Transformer · **FlashAttention y su análisis de complejidad de I/O** |
| 5 | 13–15 | Arquitecturas actuales y fenómenos | **State space models: S4, Mamba** · **Atención lineal** · **Mixture-of-experts: routing y balanceo de carga** · Double descent y benign overfitting · Lottery ticket hypothesis · Escalamiento de la profundidad |

**Prueba de Dominio.** Transformer encoder-decoder completo implementado desde cero en numpy o JAX, sin frameworks de alto nivel, con el backward pass derivado analíticamente a mano y validado con gradient checking numérico, entrenado sobre una tarea de traducción de secuencias con análisis de la curva de convergencia.

**Bibliografía.**
- **Base:** *Understanding Deep Learning* — Simon J.D. Prince (MIT Press, 2023; gratuito)
- **Complementaria:** *Deep Learning: Foundations and Concepts* — Bishop & Bishop (2023) · *Dive into Deep Learning* — Zhang et al. (gratuito). *Deep Learning* — Goodfellow, Bengio & Courville (2016) se retiene **solo como referencia histórica**: su cobertura de arquitecturas está obsoleta.
- **Papers:** *"Attention Is All You Need"* — Vaswani et al. (NeurIPS 2017) · *"Deep Residual Learning for Image Recognition"* — He et al. (CVPR 2016) · *"FlashAttention"* — Dao et al. (NeurIPS 2022) · *"Mamba: Linear-Time Sequence Modeling with Selective State Spaces"* — Gu & Dao (2023)

**Recursos.** udlbook.github.io (Prince, gratuito con notebooks) · cs231n.stanford.edu · web.stanford.edu/class/cs224n · d2l.ai · JAX y numpy únicamente para la Prueba de Dominio.

**Protocolo de estudio.** El backward pass se deriva a mano en papel para cada capa nueva **antes** de codificarla, y se valida con gradient checking numérico. Usar autograd sin haber derivado a mano al menos una vez es el atajo que vacía esta asignatura por completo.

---

