# Analysis

This folder contains all scripts, notebooks, and results for simulating and analyzing disease spread and health behavior diffusion through Social Network Exposure (SNE) and economic connectedness. The analyses focus on different epidemiological models and their response to varying levels of social interactions and network structures.

## Folder Structure
- **Code**: Contains the main scripts and notebooks for each simulation.
- **Results**: Stores the output figures generated from the simulations, organized in a subfolder named `Figures`.

## Simulation Parameters and Descriptions

### 1. `SIR.ipynb`
Implements the Susceptible-Infectious-Recovered (SIR) model, incorporating SNE to observe how social connectedness influences infection rates across socioeconomic groups.

- **Population**: 1,000 individuals
- **Initial Conditions**: 1 infected individual, 999 susceptible, 0 recovered
- **Contact Rate (β)**: 0.2
- **Recovery Rate (γ)**: 0.1 (indicating a mean recovery time of 10 days)
- **Social Network Exposure (SNE)**: Set at 1 (maximum exposure) initially, then adjusted for comparative analysis
- **Duration**: 160 days with 1-day intervals
- **Solver**: Differential equations solved using `odeint` from the `scipy.integrate` library

In regions with high SNE (low friending bias), infections spread rapidly across groups, leading to an early peak and swift decline. Lower SNE (high friending bias) localizes outbreaks, delaying the peak and extending the duration of infections.

### 2. `Age_Structured_Model.ipynb`
Models disease dynamics across two age groups, focusing on age-specific variations in infection rates and social interaction patterns.

- **Population**: 1,000 individuals, divided into young (500) and old (500)
- **Initial Conditions**: 1 infected individual per age group
- **Transmission Rates (β)**:
  - Young Group: 0.3
  - Old Group: 0.1
- **Recovery Rate (γ)**: 0.1 for both age groups (10-day recovery)
- **Social Network Exposure (SNE)**: Set at 1, indicating maximum cross-age interaction, then varied for different simulations
- **Duration**: 160 days with 1-day intervals
- **Solver**: Solved using `odeint` from `scipy.integrate`

High SNE accelerates disease spread across age groups, especially in community settings, while lower SNE results in slower, more age-segregated outbreaks.

### 3. `SLIAR.ipynb`
This model adds latent and asymptomatic compartments to the SIR framework, providing insights into undetected transmissions and asymptomatic spread.

- **Population**: 1,000 individuals
- **Initial Conditions**: 99% susceptible, 1% latent
- **Transmission Rate (β)**: 0.5
- **Infectivity Reduction for Asymptomatic (δ)**: 0.3
- **Transition Rate from Latent to Infectious (κ)**: 0.1
- **Recovery Rates**:
  - Symptomatic (α): 0.2
  - Asymptomatic (η): 0.1
- **Proportion of Latent to Symptomatic**: 0.6
- **Social Network Exposure (SNE)**: Fixed at 1.0 for full exposure, varied in simulations
- **Duration**: 160 days with 1-day intervals
- **Solver**: Solved using `odeint` from `scipy.integrate`

High SNE increases rapid transitions from susceptible to infected stages and enhances transmission among asymptomatic carriers, especially within connected socioeconomic groups.

### 4. `Clustered_Network_Epidemics.ipynb`
Simulates the effect of network clustering on disease spread, modeling a network where individuals have strong internal group connections.

- **Network Size**: 1,000 nodes
- **Triangle Connection Probability**: 0.3
- **Degree Distribution**:
  - Independent edges: Poisson distribution with mean of 2
  - Triangle edges: Poisson distribution with mean of 1
- **Infection Probability (T)**: 0.1
- **Recovery Probability**: 0.05
- **Initial Conditions**: Randomly select one node as infected
- **Clustering Coefficient (C)**: Adjusted to explore effects on infection dynamics
- **Duration**: Up to 100-time steps

A higher clustering coefficient leads to prolonged outbreaks within tightly knit groups, while lower clustering results in faster yet shorter epidemics due to fewer redundant transmission pathways.

## Usage
Each notebook contains the required libraries. Run the notebooks sequentially to explore how different parameters influence the dynamics of each model. Figures generated from the simulations are saved in the `Results/Figures` folder.

## Simulation Insights
These simulations underscore how socioeconomic connections, age-based interactions, and network clustering affect disease spread. The findings can guide public health interventions by identifying key risk factors in highly connected or segregated communities, enabling more effective containment and resource allocation strategies.
