# PTFE Crystal Structures – QE Optimized Outputs

This repository contains **Quantum ESPRESSO vc-relax outputs** for **polytetrafluoroethylene (PTFE)** in two crystalline phases:

- **Form II** – low-temperature phase (approximated as 13/6 helix)  
- **Form IV** – room-temperature phase (15/7 helix)

## Optimization Conditions

- **Code:** Quantum ESPRESSO version 7.4.1
- **Calculation type:** `vc-relax` (variable-cell relaxation with BFGS)  
- **Exchange-correlation Functional:** PBE + DFT-D3 dispersion correction  
- **Pseudopotentials:**  
C: C.pbe-n-kjpaw_psl.1.0.0.UPF  
F: F.pbe-n-kjpaw_psl.1.0.0.UPF  
- **Energy cutoffs:**  
  - Wavefunction (`ecutwfc`): 50 Ry  
  - Charge density (`ecutrho`): 300 Ry  
- **k-point mesh:** 2 × 2 × 2 (Monkhorst–Pack)  
- **Convergence thresholds:**  
  - Total energy: 1.0 × 10⁻⁵ Ry  
  - Forces: 1.0 × 10⁻⁴ Ry/Bohr  
  - Pressure: 0.1 kbar  

## Notes

- The **Form II** output reflects an approximate commensurate helix (13/6), used to model the incommensurate structure.  
- The **Form IV** output corresponds to the commensurate 15/7 helix.  
- Both are described in the **rectangular cell setting** with **two parallel chains per unit cell** and **space group P1**.

## References

- A. J. Clark, Polymer **40**, 4659–4665 (1999).  
- Quantum ESPRESSO : [https://www.quantum-espresso.org/](https://www.quantum-espresso.org/)

## Image
[IV](https://raw.githubusercontent.com/HiroYokoyama/PTFE_opt-crystal-structures/41a160e06186503134d89bd92f1c98bb9b1ab2be/img/PTFE_IV_rect_P1_twochains-vcrelax_c.png)
