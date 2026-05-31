## **IndependentCoding** 
This repository contains code to estimate the expected distribution of encoded variables based on the prevalence of every encoded variable, using neuronal encoding overlap distributions based on Fig. 3b from Engelhard et al., 2019.
## Code 
* **computational_routines.py**:
collection of functions used throughout the analysis that includes routines for probability calculations, expected distributions, biomial test, and Kolmogrov-Sirnov test.
Functions:
  * probability_k_features: gives the probability of exactly k encoded features assuming independent encoding between features
  * binomial_right_tail: calculates the right-tail probability for an observed count in a binomial distribution
  * ks_discrete_test: converts discrete values and their counts into an expanded vector representation and compares the observed and expected distibutions using two-sided K.S. test 

* **encoding_distribution_analysis.ipnyb**: main analysis notebook that loads the data and performs all calculations using computational_routines.py, statistical analysis and generates the figures. 
* Calculation of expected overlap distribution assuming independent encoding
* Comparison between observed and expected neuronal distributions
* Statistical analysis using:  
   * Binomial right-tail probabilities
   * Kolmogorv-Smirnov test
   * Geometric mean of binomial probabilities
 
## Data 
Prevalence values of encoding every variables were derived from Fig. 2a of Engelhard et al., 2019.
* prevalence of encoding for each behavioral variable are shown feature_probs.csv file 

Observed distributions were derived from Fig. 3b of Engelhard et al., 2019. 
* Observed distributions for all neurons population and for reward responsive neurons are shown in observed_counts.csv 

## To run the code 
* Download the notebook together with the required files:
  * encoding_distribution_analysis.ipynb
  * computational_routines.py
  * feature_probs.csv
  * observed_counts.csv
* Place all files in the same folder 
* Open the notebook using Jupyter Notebook
* Run all cells sequentially  
