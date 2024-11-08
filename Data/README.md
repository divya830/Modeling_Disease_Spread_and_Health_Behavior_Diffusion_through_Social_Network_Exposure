# README for Social Capital Public Data Used in the Paper by Chetty et al. (2022)

This GitHub repository provides access to four datasets on social capital in the United States, covering county, ZIP code, high school, and college levels. The datasets include aggregated measures such as economic connectedness, social cohesiveness, and civic engagement, developed through the Social Capital Atlas project by Chetty et al. (2022). These data offer insights into social capital's role in economic mobility and connectedness across different socioeconomic statuses (SES) within communities.

**Access the datasets here**: [https://www.socialcapital.org](https://www.socialcapital.org)

## Dataset Overview

1. **County-Level Data**
   - Measures include economic connectedness, childhood economic connectedness, clustering, support ratio, civic engagement, and more.
   - Population variables include the number of children with below-median parental household income and 2018 population estimates.
   - Privacy protection applied via noise addition to each metric.

2. **ZIP Code-Level Data**
   - Variables include economic connectedness, neighborhood-specific connectedness, clustering, support ratio, and civic engagement.
   - Includes population and SES-based variables similar to county-level data.
   - Protected by noise addition to ensure individual privacy.

3. **High School Data**
   - Data include economic connectedness based on own and parental SES, exposure to high-SES peers, and cohesiveness metrics.
   - Includes population data on high school student counts and ZIP code location.
   - Privacy protection through noise and cell size restrictions.

4. **College Data**
   - Contains economic connectedness measures based on SES, exposure to high-SES students, clustering, and civic engagement.
   - Data cover students per cohort and location information.
   - Noise added to protect privacy and ensure data confidentiality.

## Privacy Protection

To maintain individual privacy, these datasets use differential privacy techniques, including the addition of noise to aggregated statistics. Specific metrics, like economic connectedness and clustering, incorporate privacy-preserving mechanisms detailed in the codebook.

## Citing the Data

When using this data, please cite:

- **Chetty, R., et al. (2022a).** “Social Capital I: Measurement and Associations with Economic Mobility.” *Nature, 608*(7921), 108−121.
- **Chetty, R., et al. (2022b).** “Social Capital II: Determinants of Economic Connectedness.” *Nature, 608*(7921), 122−134.

## License

Under the terms of this License (the “License”), Meta Platforms, Inc. hereby grants, to any person or organization (“You”) obtaining a copy of this dataset and associated documentation files (the "Dataset") or otherwise accessing or using the Dataset, to use and redistribute the Dataset, with or without modification, provided that the following conditions are met:

1. Redistribution of the Dataset (or any portion of) must include and be subject to this License.
2. Neither the name of the copyright holder, nor the names of its contributors, may be used to endorse or promote products derived from this Dataset without explicit, prior written permission.
3. Use or redistribution of the Dataset must adhere to applicable laws and regulations.
4. You agree not to use the Dataset in any way (including combining the Data with other data sources) that could lead to the identification of any individual.

**Disclaimer**: THIS DATASET IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE, ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS DATASET, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
