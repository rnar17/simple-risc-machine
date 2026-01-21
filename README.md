
# 16-bit RISC Processor (Verilog)

This project implements a custom 16‑bit RISC processor written in Verilog and developed using Quartus and ModelSim. The design includes a complete datapath, ALU, instruction decoder, and an FSM‑based control unit. 

## Project Overview
The processor is based on a simple 16‑bit instruction set and a multi‑cycle execution model. The datapath, controller, and ALU were written in SystemVerilog, and their functionality was verified through simulation using ModelSim testbenches. Quartus was used for synthesis and DE1-SoC integration. 

## Main Components

### Datapath
Implements register file behavior, ALU routing, memory access, and the connections required to drive control signals.

### ALU
Provides arithmetic and logical operations required by the instruction set.

### Instruction Decoder
Extracts and interprets opcode and instruction fields that drive control logic.

### FSM Controller
Implements a multi‑cycle finite‑state machine to generate control signals for each instruction stage.

### Testbenches
Includes simulation testbenches for both the CPU and datapath (`cpu_tb.sv`, `datapath_tb.sv`) used during ModelSim verification
