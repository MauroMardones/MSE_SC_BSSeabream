# A Shortcut MSE-(Lite) Approach for Harvest Control Rule Evaluation

This repository provides a streamlined **Management Strategy Evaluation (MSE-Lite)** approach for assessing **Harvest Control Rules (HCRs)** applied to **blackspot seabream (*Pagellus bogaraveo*)**. The methodology follows the approach developed by **Henning Winker (FAO)** and is designed to evaluate quotas based on **annual benchmark stock assessment advice**.

## Authors & Contact
The methodology is based on the work of **Henning Winker** from the **Food and Agriculture Organization of the United Nations (FAO)** [Henning.Winker@fao.org](mailto:Henning.Winker@fao.org)

For more information on FAO's work related to fisheries management, visit:
[FAO Fisheries and Aquaculture](https://www.fao.org/fishery/en)


## Methodology Overview
The **FLR-based** implementation follows a simplified **Management Strategy Evaluation (MSE)** workflow tailored for blackspot seabream. The key steps include:

1. **Data Preparation**
   - Import stock assessment outputs from the annual benchmark evaluation.
   - Define initial conditions for the population model.

2. **Operating Model (OM) Setup**
   - Simulate the stock dynamics using **FLR (Fisheries Library in R)**.
   - Incorporate uncertainty in recruitment and natural mortality.

3. **Harvest Control Rule (HCR) Implementation**
   - Define candidate **HCRs** for quota setting.
   - Apply control rules iteratively based on stock status indicators.

4. **Projection & Performance Evaluation**
   - Run forward simulations under different HCR scenarios.
   - Compare performance indicators such as **long-term yield, biomass sustainability, and risk of stock collapse**.

5. **Decision Support**
   - Provide quota recommendations based on simulation outcomes.
   - Assess trade-offs between conservation and fishery objectives.

## Required Dependencies

This analysis is performed using the **FLR (Fisheries Library in R) framework**. Ensure the following R packages are installed:
```r
install.packages("FLCore")
install.packages("FLasher")
install.packages("FLAssess")
install.packages("FLBRP")
install.packages("FLFleet")
```
among others...

---

## Running the MSE Analysis
To execute the MSE simulation:
```r
# Load required libraries
library(FLCore)
library(FLasher)
library(FLAssess)
library(FLBRP)
library(FLFleet)

# Define stock and fleet objects
stock <- FLStock()
fleet <- FLFleet()

# Implement MSE projection
# (Further details should be provided based on specific model implementation)
```




