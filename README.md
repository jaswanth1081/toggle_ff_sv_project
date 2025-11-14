A simple yet essential sequential logic building block: a Toggle Flip-Flop that toggles its output on each rising clock edge only when enabled. Useful in frequency dividers, counters, and state-transition circuits.
This repository also includes a SystemVerilog testbench with interface, driver, generator, monitor, and scoreboard—providing a structured verification environment.
📌 Features
🔹 RTL Design

Toggles output (q) on positive clock edge

Controlled by enable

Active-low reset (reset_n)

Synthesizable SystemVerilog

🔹 Testbench

Interface-based DUT connection

Randomized enable signal generation

Scoreboard to compare expected vs actual output

Self-checking

Waveform dumping (dump.vcd)
.
project Structure
├── toggle_ff.sv           // RTL: Toggle Flip-Flop
├── tb_toggle_ff.sv        // Complete SV Testbench
├── dump.vcd               // Generated waveform (after simulation)
└── README.md              // Documentation
🧪 Testbench Overview

The testbench uses a verification environment including:

Interface for signal grouping

Generator – random enable patterns

Driver – drives enable into DUT

Monitor – observes outputs

Scoreboard – verifies correct toggle behavior

Environment – integrates all components
