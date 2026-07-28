### SEG-701 — Criptografía: Fundamentos Matemáticos y Protocolos — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 5 |
| **Carga** | 4–2–0 / 12 · **18 h/sem** |
| **Dificultad** | 10/10 |
| **Perfil de evaluación** | Teórico |
| **Prerrequisitos** | MAT-302, MAT-104, TEO-302 |
| **ADN institucional** | UC Berkeley CS276 · MIT 6.5620 / 18.425 *(ex 6.875)* · Stanford CS255 |

**Competencia terminal.** Construye argumentos de seguridad como reducciones formales desde una suposición computacional, y detecta cuándo un esquema carece de ese argumento.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Marco formal | Juegos de seguridad · Ventaja del adversario · Seguridad perfecta (one-time pad) vs computacional · Funciones de un solo sentido (OWF) como suposición central · Predicados hardcore |
| 2 | 4–6 | Primitivas simétricas | PRG: stretch e indistinguibilidad · PRF: construcción desde PRG por árbol GGM · PRP y cifrados de bloque · AES y su análisis algebraico en GF(2⁸) (conexión con MAT-302) · Modos de operación · MAC y HMAC · Cifrado autenticado (AEAD) |
| 3 | 7–9 | Nociones de seguridad y clave pública | IND-CPA, IND-CCA1, IND-CCA2 · Relaciones entre nociones · RSA y su análisis (OAEP) · ElGamal · Diffie-Hellman: suposiciones CDH y DDH · Curvas elípticas: grupo de puntos sobre GF(p), ECDLP, ECDSA, EdDSA |
| 4 | 10–12 | Hash y pruebas de conocimiento | Modelo del oráculo aleatorio y sus límites · Resistencia a colisiones · Merkle-Damgård vs esponja (SHA-3/Keccak) · Zero-knowledge: completitud, solidez, ZK por simulación · Protocolos sigma · Fiat-Shamir · Compromisos · Oblivious Transfer |
| 5 | 13–15 | Criptografía post-cuántica y avanzada | **Problemas reticulares: SIS, LWE, Ring-LWE** · **Estándares NIST: ML-KEM (FIPS 203), ML-DSA (FIPS 204), SLH-DSA (FIPS 205)** · Firmas basadas en hash · **Encriptación completamente homomórfica: BGV, CKKS, bootstrapping** · Computación multipartita segura (introducción) |

**Prueba de Dominio.** Demostración formal de que ningún cifrado de clave pública puede ser IND-CCA2 sin padding apropiado (con el ataque explícito como contraejemplo constructivo) + construcción de un protocolo de identificación Σ con demostración de las tres propiedades, incluyendo el simulador explícito para zero-knowledge.

**Bibliografía.**
- **Base:** *A Graduate Course in Applied Cryptography* — Boneh & Shoup (gratuito)
- **Complementaria:** *Introduction to Modern Cryptography* (3ª ed.) — Katz & Lindell · *Foundations of Cryptography* Vol. 1–2 — Goldreich · *Serious Cryptography* (2ª ed.) — Aumasson (perspectiva de implementación)
- **Estándares:** FIPS 197 (AES) · FIPS 202 (SHA-3) · FIPS 203/204/205 (post-cuántica)
- **Papers:** *"New Directions in Cryptography"* — Diffie & Hellman (1976) · *"On Lattices, Learning with Errors..."* — Regev (JACM 2009)

**Recursos.** toc.cryptobook.us (Boneh & Shoup gratuito) · crypto.stanford.edu/~dabo/courses/cs255 · csrc.nist.gov/projects/post-quantum-cryptography · CryptoHack y cryptopals para práctica de ataques · SageMath para aritmética de curvas y retículos.

**Protocolo de estudio.** Toda prueba de seguridad se escribe como reducción explícita: *adversario que rompe el esquema → adversario que rompe la suposición*. Formato de tarjeta único de la asignatura: "dado este esquema roto, construye el adversario contra la suposición subyacente". Memorizar el enunciado de seguridad sin la reducción no sirve para nada en esta asignatura.

---

