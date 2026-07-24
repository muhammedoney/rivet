---
name: rivet-bfm-sim
description: Wire Vivado Root Port or Endpoint BFM into Questa alongside Rivet DUT. Use for tb/bfm side-path work, not as a replacement for UVM.
---

# Rivet BFM sim skill

1. Read `tb/bfm/README.md`.
2. Export Vivado RP BFM (for EP `MODE`) or EP BFM (for RC `MODE`) into local `third_party/bfm/` (gitignored).
3. Connect BFM to `rivet_pcie_ctrl` or full `rivet_pcie`; keep scripts under `tb/bfm/`; do not commit proprietary binaries.
4. Treat failures as complementary evidence; still track DUT bugs in UVM tests when applicable.
5. Record Vivado version and export steps in docs when first successful.
