# Plant Phenotype Prediction in Arabidopsis thaliana
This project was conducted as part of the "**Artificial Intelligence for Biotechnology**" course at **Technical University of Munich, Straubing Campus**. The goal was to develop a predictive model capable of forecasting the **phenotypic responses** of individual plants based on their genetic variations.
We utilized genomic data from the **1001 Genomes Project for Arabidopsis thaliana**, which contains whole-genome sequencing data of Arabidopsis thaliana samples, identifying genetic variations among them (Alonso-Blanco et al., 2016). For this study, **5000 single nucleotide polymorphisms (SNPs)** were selected, and we created an in silico phenotype related to biomass as our dataset. The biomass for each plant was quantified in grams (g).

# Approach
## 1. Data Preprocessing
* Data Imputation for missing values
* Ensured equal sample size for genotype & phenotype data
* Additive Encoding for genotype data
* Initial Data Visualization
## 2. Model Selection
We tested multiple regression models:
* LASSO Regression
* Support Vector Regression (SVR)
* Polynomial Kernel
* RBF Kernel
* Nu-SVR
* K-Nearest Neighbors Regression (KNR)
* Kernel Ridge Regression (KRR)
* Tweedie Regression (TR)
* Bayesian Ridge Regression <br />
Additionally, we adopted regularization (C and alpha tuning) and feature selection methods

# Results
## Performance of Tested Models on unseen data 
**Model**  |  **MSE**  | Explained Variance
------------- | ------------- | -------------
LASSO  | 4.33 | 0.53
SVR (Polynomial)  | 5.16 | 0.44
SVR (RBF)  | 5.16 | 0.44
KRR  | 4.66 | 0.50
KNR  | 7.75 | 0.23
BR  | 4.69 | 0.50
TR  | 4.72 | 0.50

# How to Run the Project
## Requirements
Ensure you have the following dependencies installed:
```
pip install numpy pandas scikit-learn matplotlib jupyter
```
## Step
1. Clone the repository:
```
git clone https://github.com/ashi198/Plant-Phenotype-Prediction-in-Arabidopsis-thaliana.git
cd Plant-Phenotype-Prediction
```
2. Open code_file.ipynb to execute the cells and get to know more about the project

# Citation
Alonso-Blanco, Carlos, et al. "1,135 genomes reveal the global pattern of polymorphism in Arabidopsis thaliana." Cell 166.2 (2016): 481-491.

# Acknowledgments
Special thanks to TUM Straubing Campus and the Artificial Intelligence for Biotechnology course instructors for their guidance and support.
