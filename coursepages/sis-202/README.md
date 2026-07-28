### SIS-202 — Circuitos Digitales y Diseño Lógico

| | |
|---|---|
| **Créditos** | 4 |
| **Carga** | 2–0–4 / 8 · **14 h/sem** |
| **Dificultad** | 8/10 |
| **Perfil de evaluación** | Sistemas |
| **Prerrequisitos** | MAT-101 |
| **ADN institucional** | MIT 6.1910 *(ex 6.004)* · CMU 18-240 |

**Competencia terminal.** Sintetiza un procesador funcional desde la especificación de su ISA, con análisis de temporización correcto.

**Unidades**

| # | Sem. | Unidad | Contenido |
|---|---|---|---|
| 1 | 1–3 | Álgebra de conmutación | Axiomas de Huntington · Formas canónicas · Minimización · Mapas de Karnaugh · Quine-McCluskey |
| 2 | 4–6 | Lógica combinacional | Multiplexores, decodificadores, codificadores · Sumadores: ripple-carry, carry-lookahead · ALU · Análisis de retardo de propagación |
| 3 | 7–9 | Lógica secuencial y FSM | Latches y flip-flops D/JK/T · Máquinas de Moore vs Mealy · Síntesis de FSM · Codificación de estado, one-hot · Metaestabilidad |
| 4 | 10–12 | HDL y flujo de diseño | SystemVerilog: síntesis vs simulación · Testbenches · RTL → síntesis lógica → place-and-route · FPGAs: LUTs, routing |
| 5 | 13–15 | Temporización y microarquitectura | Setup/hold, slack, static timing analysis · Camino crítico · Pipelining del datapath · Forwarding y detección de hazards en hardware |

**Prueba de Dominio.** Procesador RISC-V RV32I en SystemVerilog con pipeline de 5 etapas, forwarding de datos, detección de hazards y predictor de saltos, sintetizable en FPGA, validado contra un banco de pruebas de conformidad de la ISA.

**Bibliografía.**
- **Base:** *Digital Design and Computer Architecture: RISC-V Edition* (2ª ed.) — Harris & Harris
- **Complementaria:** *Computer Organization and Design: RISC-V Edition* — Patterson & Hennessy · *Nand2Tetris* (Nisan & Schocken) como puente conceptual
- **Especificación:** *The RISC-V Instruction Set Manual, Volume I: Unprivileged ISA* (versión ratificada vigente)

**Recursos.** MIT OCW 6.004 · riscv.org (especificaciones oficiales) · Verilator, Icarus Verilog, GTKWave · Ripes (simulador visual de RISC-V) · riscv-tests para conformidad.

**Protocolo de estudio.** Simulación antes de síntesis; testbench antes de diseño. El *waveform* se predice en papel antes de mirarlo — el hábito de leer la forma de onda para descubrir qué hace el circuito impide entenderlo.

---

