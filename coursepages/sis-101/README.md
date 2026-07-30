### SIS-101 — Programación Científica y Sistemas — **[NÚCLEO]**

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 7/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | ∅ |
| **ADN institucional** | CMU 15-122 · MIT 6.1010 *(ex 6.009)* |

**Competencia terminal.** Escribe código C correcto por contrato, con invariantes de representación explícitas y gestión manual de memoria verificada.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Modelo de ejecución | Stack, heap, registros · Ciclo de compilación y enlazado · Tipos como contratos formales |
| 2 | 4–6 | Contratos e invariantes | Precondiciones y postcondiciones · Invariante de representación · Invariante de abstracción · Aserciones ejecutables |
| 3 | 7–9 | Recursión y terminación | Recursión estructural · Medida de terminación · Recursión de cola · Conversión a iteración con invariante preservado |
| 4 | 10–12 | Memoria manual | malloc/free · Punteros y aritmética de punteros · Arrays multidimensionales: row-major vs column-major · Fugas, use-after-free, double free · valgrind |
| 5 | 13–15 | Depuración a bajo nivel | GDB: breakpoints, watchpoints, inspección de memoria · Lectura de desensamblado · Sanitizers (ASan, UBSan) |

**Laboratorios.** L1 arreglos con contratos · L2 listas enlazadas con invariante · L3 tablas hash · L4 depuración de código sembrado con errores · L5 perfilado de memoria.

**Prueba de Dominio.** Slab allocator en C con free-list, coalescing de bloques libres y demostración formal de la invariante de representación mediante contratos anotados. Sometido a inyección de patrones de asignación adversariales.

**Contabilidad de costo (§15.8).** Se acota cómputo y memoria del allocator —costo por operación y fragmentación— y se declara su escalamiento respecto al número y tamaño de las asignaciones, contrastado contra la complejidad derivada.

**Bibliografía.**
- **Base:** *C Programming: A Modern Approach* (2ª ed.) — K.N. King
- **Complementaria:** *The C Programming Language* — Kernighan & Ritchie · *Modern C* — Gustedt (gratuito)
- **Papers:** —

**Recursos.** CMU 15-122 (sitio público con labs) · Harvard CS50x para nivelación previa · Compiler Explorer (godbolt.org) para inspeccionar el código generado.

**Protocolo de estudio.** *Predict-then-verify* obligatorio: antes de ejecutar, escribes el estado esperado de la memoria; luego lo verificas en GDB. Cada divergencia genera una tarjeta de traza.

---

