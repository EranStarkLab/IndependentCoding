## **IndependentCoding** 
This repository contains code to estimate the expected distribution of encoded variables based on the prevalence of every encoded variable.
## Code 
* **computational_routines.py:**\
A collection of functions used throughout the analysis that includes routines for probability calculations, expected distributions, binomial test, and Kolmogrov-Smirnov test.
   * Functions:
       * probability_k_features: calculates the probability of exactly k encoded features assuming independent encoding between features
       * binomial_right_tail: calculates the right-tail probability for an observed count in a binomial distribution
       * ks_discrete_test: converts discrete values and their counts into an expanded vector representation and compares the observed and expected distributions using a two-sided Kolmogorov-Smirnov test 

* **encoding_distribution_analysis.ipnyb:**\
Main analysis notebook that loads the data, calls functions from computational_routines.py, performs statistical analyses, and generates the figures.
  * The notebook includes:
       * Calculation of expected overlap distribution assuming independent encoding
       * Comparison between observed and expected neuronal distributions
       * Statistical analyses using:  
          * Binomial right-tail probabilities
          * Kolmogorov-Smirnov test
          * Geometric mean of binomial probabilities
 
## Data 
* **observed_neurons.csv:**\
Contains the prevalence of encoding for each behavioral variable, derived from Fig. 2a of Engelhard et al., 2019.  
* **observed_counts.csv**:\
Contains the observed numbers of encoding 0-5 variables for the all neurons population and the reward responsive neurons subset, derived from Fig. 3b of Engelhard et al., 2019.

## To run the code 
* Download the notebook together with the required files:
  * encoding_distribution_analysis.ipynb
  * computational_routines.py
  * observed_neurons.csv
  * observed_counts.csv
* Place all files in the same folder 
* Open the notebook using Jupyter Notebook
* Run all cells sequentially  
