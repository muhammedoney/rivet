---
name: rivet-phy-wrapper
description: Add or adjust Rivet FPGA-family PCIe PHY wrappers (PG239) and rivet_pcie top. Use when editing rtl/phy or rtl/top or integrating Xilinx PHY.
---

# Rivet PHY skill

1. Preserve PIPE-only boundary to `rivet_pcie_ctrl`.
2. Add family modules beside `rivet_pcie_phy_usplus` / `rivet_pcie_phy_us`.
3. Wire through `rivet_pcie` generate / `FPGA_FAMILY`.
4. Never commit encrypted Xilinx IP; keep stubs + generation notes.
5. Keep `LANES` in {1,2,4} consistent with the controller.
