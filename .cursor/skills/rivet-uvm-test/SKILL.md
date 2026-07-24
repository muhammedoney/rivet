---
name: rivet-uvm-test
description: Add or extend Rivet UVM tests, sequences, agents, scoreboard, and coverage. Use when working under tb/uvm or when the user asks for new UVM tests.
---

# Rivet UVM test skill

1. Read `docs/verification.md` and existing `tb/uvm/` agents/env/tests.
2. Keep DUT as **`rivet_pcie_ctrl`**; set `LANES` via `RIVET_TB_LANES` / config DB.
3. Prefer extending stubs over restructuring env hierarchy.
4. New smoke tests: follow `smoke_gen2_x1` / `x2` / `x4` naming.
5. Update `rivet_uvm_pkg.sv` includes and `filelist_uvm.f` if new files are added.
6. Document how to run with `scripts/sim_questa.*`.
