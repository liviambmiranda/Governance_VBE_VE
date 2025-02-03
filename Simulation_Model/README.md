# Overview
This repository contains Python codes that simulate voting processes (shared decision-making) in a network of members (or firms). The simulation introduces concepts like quorum requirements and token-based incentives (representing voting power) for firms' participation. The simulation outputs analyse power imbalance and quorum attainment (administrative efficiency in shared decision-making) across multiple voting rounds.

---

## Table of Contents :memo:

1. [Requirements](#requirements)  
2. [Key Features](#key-features)  
3. [Simulation Details](#simulation-details)  
4. [How to Run](#how-to-run)  
5. [Example Output](#example-output)  
6. [Notes](#notes)  

---

## Requirements :wrench:

- **Python 3.7+**  
- **Matplotlib** (for visualizations)  

Install the required package via:

    pip install matplotlib

## Key Features :star:

1.  **Voting Simulations**:
    
    -   Members probabilistically vote across multiple rounds.
    -   Different quorum thresholds (e.g., 50%, 70%, 80%, 90%) are analysed.
2.  **Token Reward Mechanism**:
    
    -   Tokens are awarded to members based on participation in voting rounds.
    -   Configurable token rewards (e.g., 1, 2, or 3 tokens per round).
3.  **Power Imbalance Analysis**:
    
    -   Tracks the distribution of tokens (representing voting power) among members to measure power disparities over time.
    
4.  **Administrative Efficiency Analysis**:
    
    -   Tracks the frequency of quorum attainment across voting rounds and varying quorum thresholds.
    
5.  **Visualization**:
    
    -   Generates graphs for power imbalance, administrative efficiency, and total token distribution.

----------

## Simulation Details :bulb:

1.  **Network Setup**:
    
    -   A network of members is initialised, where each member:
        -   Votes probabilistically (e.g., 80% chance of voting).
        -   Earns tokens as a reward for participation.
        -   Has unique tracking for token counts and voting behaviour.
2.  **Voting Rounds**:
    
    -   Multiple voting rounds are simulated.
    -   Members’ votes are reset for each round.
    -   Quorum attainment is checked, and rewards are distributed if the quorum is met.
3.  **Metrics Tracked**:
    
    -   **Power Imbalance**: Difference between the most and least rewarded members.
    -   **Administrative Efficiency**: Number of rounds in which quorum was achieved.
    
4.  **Visualization**:
    
    -   Graphs are generated for:
        -   Power imbalance across rounds.
        -   Administrative efficiency vs. quorum percentage.
        -   Total token distribution across rounds.

----------

## How to Run :checkered_flag:

1.  **Clone or Download** this repository.
2.  **Set Simulation Parameters**:
    -   Adjust `quorums` to test different quorum thresholds (e.g., `[0.5, 0.7, 0.8, 0.9]`).
    -   Set token rewards in `tokens_added_values` (e.g., `[1, 2, 3]`).
    -   Modify voting probabilities in the `gerar_voto` method if needed.
3.  **Run the Scripts**:
    -   Execute the Python scripts in your preferred environment.
4.  **View Results**:
    -   Graphs will be saved as PDFs in the working directory.

----------

## Example Output :bar_chart:

1.  **Power Imbalance**:
    
    -   **Graph**: Tracks the difference in tokens between the most and least rewarded members across rounds.
    -   **X-axis**: Voting Rounds.
    -   **Y-axis**: Power Imbalance.
2.  **Administrative Efficiency**:
    
    -   **Graph**: Scatter plot of voting rounds achieving quorum at various thresholds.
    -   **X-axis**: Quorum Percentage (%).
    -   **Y-axis**: Number of Voting Rounds Achieving Quorum.


----------

## Notes :bulb:

-   **Customization**:
    -   Adjust `quantidade_membros` in the `Rede` class to simulate networks of different sizes.
    -   Modify the voting probabilities in the `gerar_voto` method to reflect different participation behaviours.
-   **Graph Outputs**:
    -   Graphs are saved as:
        -   `amplitude_quorum_<quorum>.pdf` for power imbalance.
        -   `quorum_atingido_10000_iteracoes_scatter.pdf` for quorum attainment.
    
