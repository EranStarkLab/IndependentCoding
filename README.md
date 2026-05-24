## **IndependentCoding** 
This repository contains code to estimate the expected distribution of encoded variables based on the prevalence of every encoded variable, using neuronal encoding overlap distributions based on Fig. 3b from Engelhard et al., 2019.
## Code 
encoding_distribution_analysis.ipnyb
##
* Calculation of expected overlap distribution assuming independent encoding
* Comparison between observed and expected neuronal distributions
* Statistical analysis using:  
   * Binomial right-tail probabilities
   * Kolmogorv-Smirnov test
   * Geometric mean of binomial probabilities

* probability_k_feature: 
## Data 
Prevalence values of encoding every variables were derived from Fig. 2a of Engelhard et al., 2019.
* Total neuron population: 303
* Position: 91/303
* Kinematics: 137/303
* Cues: 77/303
* Accuracy: 69/303
* Previous reward: 95/303
* Reward response: 232/303

Observed distributions were derived from Fig. 3b of Engelhard et al., 2019. 
* Observed distributions for all neurons population:
  * 0 variables: 47 neurons
  * 1 variable: 105 neurons
  * 2 variables: 103 neurons
  * 3 variables: 40 neurons
  * 4 variables: 6 neurons
  * 5 variables: 2 neurons

* Observed distributions for reward responsive neurons:
  * 0 variables: 30 neurons
  * 1 variable: 84 neurons
  * 2 variables: 77 neurons
  * 3 variables: 35 neurons
  * 4 variables: 5 neurons
  * 5 variables: 1 neuron

## To run the code 
* Download the notebook together with the required '.csv' files:
  * feature_probs.csv
  * observed_counts.csv
* Place all files in the same folder 
* Open the notebook using Jupyter Notebook
* Run all cells sequentially  
