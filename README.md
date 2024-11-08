# Modeling Disease Spread and Health Behavior Diffusion through Social Network Exposure and Connectedness

## Project Overview
This project investigates how social network structures and economic connectedness affect infectious disease spread and health behavior diffusion. 
This repository contains all materials for my project exploring the dynamics of infectious disease transmission influenced by social network structures and demographic factors. The project incorporates modified epidemiological models, integrating Social Network Exposure (SNE) and clustering effects to understand disease spread and health behavior diffusion across different socioeconomic groups and age structures. Key analyses include economic connectedness, age-structured transmission, the SLIAR model with social exposure, and clustered network effects on infection rates.
The project draws upon foundational concepts from two key papers by Raj Chetty et al. on Social Capital:
Social Capital I: Measurement and Associations with Economic Mobility
Social Capital II: Determinants of Economic Connectedness
The repository includes data, code, results, as well as the final report and presentation, organized to facilitate understanding of results.

## Repository Structure
- **Data**  
  Contains the data files and links to the datasets used in base papers.
  - `README.md`: Information on the data sources and structure.
  - `social_capital_county.csv`: Measures include economic connectedness, childhood economic connectedness, clustering, support ratio, civic engagement, and more.
  - `social_capital_zip.csv`: Variables include economic connectedness, neighborhood-specific connectedness, clustering, support ratio, and civic engagement.
  - `social_capital_high_school.csv`: Data include economic connectedness based on own and parental SES, exposure to high-SES peers, and cohesiveness metrics.
  - `social_capital_college.csv`: Contains economic connectedness measures based on SES, exposure to high-SES students, clustering, and civic engagement.
  
- **Analysis**  
  Contains all scripts and notebooks used to perform the analyses.
  - `README.md`: Descriptions of each analysis script and its purpose.
  - **Code**
  - Contain Python scripts for all simulations.
    - `SIR.ipynb`: Python script for the SIR model and the effect of change in SNE (Social Newtork Exposure).
    - `Age_Structured_Model.ipynb`: Python script for the Age Structured Model and the effect of change in SNE (Social Newtork Exposure).
    - `SLIAR.ipynb`: Python script for the SLIAR Model and the effect of change in SNE (Social Newtork Exposure).
    - `Clustered_Network_Epidemics.ipynb`: Python script for Clustered Network Epidemics via Incorporating Social Interactions
  - **Results**
    - `Figures`: Folder for all figures in the result after simulation.

- **Report Folder**  
  Contains the report and associated files.
  - `Figures`: Folder for images and figures included in the report.
  - `Report.tex`: LaTeX source file for the report.
  - `Report.pdf`: Compiled final report in PDF format.
  - `Bibliography.bib`: BibTeX file for references used in the report.
  
- **Slides**  
  Contains the presentation materials.
  - `Presentation.pdf`: Final presentation in PDF format.
  - `Source_file.pptx`: Source File for Final Presentation.
  
- **Base Papers Summary Slides**  
  - `Base_Paper_1.pdf`: Paper 1 in PDF format.
  - `Base_Paper_2.pdf`: Paper 2 in PDF format.
  - `Presentation_1.pdf`: Presentation of Paper 1 in PDF format.
  - `Presentation_2.pdf`: Presentation of Paper 2 in PDF format.
  - `Source_file1.pptx`: Source File for Presentation of Paper 1.
  - `Source_file2.pptx`: Source File for Presentation of Paper 2.

## Project Analyses
The project consists of four main analyses:
1. **Economic Connectedness and Disease Spread**  
   Examines the role of economic ties in disease transmission using the modified SIR model with SNE.

2. **Age-Structured Models for Disease Dynamics**  
   Uses age-specific parameters in a modified SIR model to understand how demographic factors influence spread and recovery.

3. **SLIAR Model with Social Network Exposure (SNE)**  
   Extends the SIR model to include latent and asymptomatic stages, with SNE affecting disease dynamics.

4. **Clustered Network Epidemics**  
   Analyzes how social clustering and interactions within close-knit communities affect epidemic spread using network-based simulations.

## Key Findings
- Social network exposure and economic connectedness accelerate disease transmission across social classes.
- Age-specific contact rates and recovery rates significantly affect infection peaks and spread dynamics.
- High clustering coefficients in network structures sustain infections within tightly connected groups.

## Usage Instructions
1. Clone this repository to access data, code, and supplementary files.
2. Follow instructions in the `Analysis` folder's `README.md` to replicate simulations or customize parameters for your research.
3. View the `Report.pdf` for a detailed analysis and findings summary.

## License
This work is licensed under a Creative Commons Attribution-NonCommercial 4.0 International License. You are free to share and adapt the materials for non-commercial purposes with proper attribution.

