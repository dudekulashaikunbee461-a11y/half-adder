# Half Adder using Verilog

## Project Overview

A Half Adder is a combinational logic circuit used to add two single-bit binary numbers.
It has two inputs (A and B) and two outputs:

- Sum (S)
- Carry (C)

This project implements a Half Adder in Verilog HDL and verifies its functionality using a testbench.

---

## Truth Table

| A | B | Sum | Carry |
|---|---|-----|-------|
| 0 | 0 |  0  |   0   |
| 0 | 1 |  1  |   0   |
| 1 | 0 |  1  |   0   |
| 1 | 1 |  0  |   1   |

---

## Logic Equations

Sum = A XOR B

Carry = A AND B

---

## Files

| File | Description |
|------|-------------|
| half_adder.v | Verilog source code |
| half_adder_tb.v | Testbench |
| simulation_output.png | Simulation waveform |
| README.md | Project documentation |

---

## Software Required

- Xilinx Vivado
- ModelSim
- Icarus Verilog
- GTKWave

---

## How to Run

1. Compile the design

```
iverilog -o half_adder half_adder.v half_adder_tb.v
```

2. Run simulation

```
vvp half_adder
```

3. View waveform

```
gtkwave half_adder.vcd
```

---

## Expected Output

```
A=0 B=0 Sum=0 Carry=0
A=0 B=1 Sum=1 Carry=0
A=1 B=0 Sum=1 Carry=0
A=1 B=1 Sum=0 Carry=1
```

---

## Author

Sai Pallavi

B.Tech ECE
