### TEO-401 — Teoría de la Información y Códigos

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 3–2–0 / 9 · **14 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-104, MAT-302 |
| **ADN institucional** | MIT 6.441[J] · Stanford EE376A |

**Competencia terminal.** Deriva la capacidad de un canal y construye códigos que se aproximen a ella, cuantificando la brecha.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Medidas de información | Entropía H(X) · Entropía conjunta y condicional · Información mutua I(X;Y) · Divergencia KL · Desigualdad de procesamiento de datos · Desigualdad de Fano |
| 2 | 4–6 | Codificación de fuente | Códigos de prefijo · Desigualdad de Kraft · Huffman y su optimalidad · Codificación aritmética · Primer Teorema de Shannon · AEP y conjuntos típicos |
| 3 | 7–9 | Capacidad de canal | Definición C = max I(X;Y) · Canal simétrico binario · Segundo Teorema de Shannon con demostración por codificación aleatoria · Recíproco · Canal gaussiano: C = ½ log(1+SNR) |
| 4 | 10–12 | Códigos correctores | Distancia de Hamming · Cotas: Singleton, Hamming, Gilbert-Varshamov · Códigos lineales: matriz generadora y de paridad, código dual · Códigos cíclicos: BCH · Reed-Solomon sobre GF(2ⁿ) |
| 5 | 13–15 | Códigos modernos y complejidad | LDPC y sum-product (belief propagation) · Códigos polares (introducción) · Teorema de Slepian-Wolf · Complejidad de Kolmogorov · MDL · Incompresibilidad y su uso como método de prueba |

**Prueba de Dominio.** Demostración completa del Teorema de Codificación de Canal (existencia de códigos aleatorios que alcanzan la capacidad) + implementación de codificador y decodificador Reed-Solomon con el algoritmo de Berlekamp-Welch, medido sobre canal simulado con la brecha respecto a la capacidad cuantificada.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del codificador y del decodificador y se declara su escalamiento respecto a la longitud del bloque y a la capacidad de corrección, contrastado contra la complejidad derivada.

**Bibliografía.**
- **Base:** *Elements of Information Theory* (2ª ed.) — Cover & Thomas
- **Complementaria:** *Information Theory, Inference, and Learning Algorithms* — MacKay (gratuito) · *Essential Coding Theory* — Guruswami, Rudra & Sudan (borrador gratuito)
- **Papers:** *"A Mathematical Theory of Communication"* — Shannon (Bell System Technical Journal, 1948)

**Recursos.** inference.org.uk/mackay/itila (MacKay completo, gratuito) · Stanford EE376A · Galois field libraries para validar la aritmética de MAT-302.

**Protocolo de estudio.** Las cotas de Shannon se contrastan siempre contra códigos reales implementados. La brecha entre cota y práctica es el objeto de estudio de la unidad 5, no un defecto de la implementación.

---

