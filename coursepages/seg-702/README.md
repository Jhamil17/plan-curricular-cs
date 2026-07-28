### SEG-702 — Seguridad de Sistemas y Ataques a Bajo Nivel

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 9/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | SIS-201, SIS-501 |
| **ADN institucional** | CMU 15-330 · UC Berkeley CS161 · Stanford CS155 |

**Competencia terminal.** Construye un modelo de amenaza explícito y deriva de él tanto el ataque como la mitigación.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelado de amenaza | Definición de adversario y de sus capacidades · Superficie de ataque · Trust boundaries · Principios de diseño seguro (Saltzer & Schroeder) · Análisis de riesgo |
| 2 | 4–6 | Vulnerabilidades de memoria | Buffer overflow en stack y heap · Use-after-free · Double free · Format string · Integer overflow · Explotación: control de RIP, shellcode |
| 3 | 7–9 | Mitigaciones y evasión | DEP/NX · Stack canaries · ASLR y PIE · CFI · Return-oriented programming · Formato ELF, PLT/GOT, lazy binding · Bypass de cada mitigación |
| 4 | 10–12 | Canales laterales y protocolo | Timing attacks sobre RSA · Cache-timing: Flush+Reload, Prime+Probe · Spectre y Meltdown: análisis microarquitectural · Padding oracle · BEAST, CRIME · Bleichenbacher sobre PKCS#1 · Criptoanálisis diferencial y lineal |
| 5 | 13–15 | Análisis y modelos formales | Fuzzing guiado por cobertura (AFL++) · Ejecución simbólica y concólica (KLEE, angr) · Ingeniería inversa: estático vs dinámico · SQL injection, XSS, CSRF, SSRF a nivel de protocolo · Bell-LaPadula y Biba con demostración de propiedades |

**Prueba de Dominio.** Explotación completa de un binario Linux x86-64 con PIE, ASLR y stack canaries activos, mediante cadena ROP construida desde primeros principios (sin herramientas automáticas de generación de cadenas) + demostración matemática del ataque de padding oracle, explicando por qué CBC sin autenticación es estructuralmente inseguro.

**Bibliografía.**
- **Base:** *Computer Security: Art and Science* (2ª ed.) — Bishop
- **Complementaria:** *The Art of Software Security Assessment* — Dowd, McDonald & Schuh · *Practical Binary Analysis* — Andriesse · *The Shellcoder's Handbook*
- **Papers:** *"Smashing the Stack for Fun and Profit"* — Aleph One (Phrack 49, 1996) · *"Spectre Attacks: Exploiting Speculative Execution"* — Kocher et al. (S&P 2019) · *"The Protection of Information in Computer Systems"* — Saltzer & Schroeder (1975)

**Recursos.** pwn.college (curso estructurado de explotación) · picoCTF · Ghidra, radare2, pwntools, GDB con pwndbg · AFL++, KLEE, angr · **Máquina virtual aislada obligatoria.**

**Protocolo de estudio.** Trabajo exclusivamente sobre binarios y entornos propios, aislados en máquina virtual sin red. La asignatura se estudia **desde el modelo de amenaza hacia el exploit**, nunca al revés: memorizar técnicas sin modelo produce operadores de herramientas, no investigadores de seguridad.

---

