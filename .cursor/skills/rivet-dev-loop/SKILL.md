---
name: rivet-dev-loop
description: Run Rivet verification loop after RTL/TB changes — Verilator lint/smoke, optional Yosys, Questa UVM when available. Use after coding slices or when the user asks to verify or loop.
---

# Rivet dev loop

1. From repo root, run Verilator lint: `scripts/lint.ps1` (Windows) or `scripts/lint.sh`.
2. Optionally run Verilator smoke build: `scripts/sim_verilator.ps1` / `.sh`.
3. If `vsim` is available, run `scripts/sim_questa.ps1 smoke_gen2_x1`.
4. Optionally Yosys: `scripts/synth_yosys.sh`.
5. Summarize pass/fail; fix failures before the next feature slice.
6. If Questa is missing, say so and continue with Verilator as the gate.
