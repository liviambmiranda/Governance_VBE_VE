# Overview
This repository contains a Python code designed to analyze **operational validity** through a **parameter variability-sensitivity analysis**. The analysis focuses on varying the participation probability of firms within a simulation-based voting model, examining its effects, e.g. on **power imbalance** across multiple voting rounds under different quorum and reward structures.

---

## Key Features :star:

1. **Participation Probability Variability**:
   - Simulates firms’ participation with adjustable probabilities (e.g., 90%, 80%, 70%, etc.).
   - Analyzes how changes in participation rates affect the power distribution in shared decision-making.

3. **Graphical Visualization**:
   - Power imbalance results are visualized to highlight the effects of different participation probabilities.

---


## How to Run :checkered_flag:

1. **Set Up Participation Probabilities**:
   - Modify the `gerar_voto` method in the `Membro` class to adjust participation probabilities (e.g., 90%, 80%, 70%, etc.).

2. **Run the Simulation**:
   - Define quorum thresholds and token rewards:
     - Quorums: `[0.5, 0.7, 0.8, 0.9]`.
     - Token Rewards: `[1, 2, 3]`.
   - Execute the script in a Python environment.

3. **View Results**:
   - Graphs for each quorum and token reward configuration will be saved as PDFs.
