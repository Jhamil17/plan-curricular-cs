### INT-400 — Laboratorio Integrador IV

| | |
|---|---|
| **Créditos** | 2 |
| **Carga** | 0–0–3 / 5 · **8 h/sem** |
| **Perfil de evaluación** | Investigación |
| **Prerrequisitos** | ALG-403, TEO-401, MAT-302 (concurrentes) |

**Artefacto.** Codificador/decodificador Reed-Solomon paralelizado, con: (a) aritmética de GF(2⁸) implementada desde la construcción algebraica de MAT-302, (b) paralelización con análisis exacto de trabajo y span según ALG-403, (c) medición de escalabilidad contra la predicción de la ley de Brent, con la discrepancia atribuida a componentes específicos (contención, false sharing, overhead de planificación), (d) verificación de la tasa de corrección contra la cota de Singleton sobre canal simulado.

**Integra:** MAT-302 (cuerpos finitos) + TEO-401 (códigos y capacidad) + ALG-403 (paralelismo y análisis W/S) + ALG-401 (análisis de complejidad).

**Defensa oral.** 20 minutos: explicar por qué la escalabilidad medida se desvía de la predicción teórica, con evidencia de perfilado.
---

# CICLO V — Sistemas Complejos: SO, Compiladores, Redes y Bases de Datos

**25 créditos · 26 h lectivas/sem · 28 h EI/sem · Total ≈54 h/sem**

> **Propósito del ciclo.** El ciclo de mayor carga de construcción del programa. Cuatro sistemas completos se escriben desde cero en paralelo, y una asignatura de métodos formales verifica propiedades de los otros tres. Aquí la malla deja de ser asignaturas paralelas y se convierte en una pila: el compilador genera código para el kernel, y el verificador demuestra que el planificador no bloquea.

---

