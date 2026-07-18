## **IndependentCoding** 
This repository contains code to estimate the expected distribution of encoded variables based on the prevalence of every encoded variable.
## Code 
* **computational_routines.py:**\
A collection of functions used throughout the analysis that includes routines for probability calculations, expected distributions, binomial test, and Kolmogrov-Smirnov test.
   * Functions:
       * probability_k_variables: calculates the probability of exactly k encoded variables assuming independent encoding between variables
       * binomial_right_tail: calculates the right-tail probability for an observed count in a binomial distribution
       * ks_discrete_test: converts discrete values and their counts into an expanded vector representation and compares the observed and expected distributions using a two-sided Kolmogorov-Smirnov test
       * peak_properties: calculates the prevalence that produces the largest number of neurons encoding exactly one variable and the probability of encoding exactly one variable at that prevalence

* **encoding_distribution_analysis.ipnyb:**\
Main analysis notebook that loads the data, calls functions from computational_routines.py, performs statistical analyses, and generates the figures.
  * The notebook includes:
       * Calculation of expected overlap distribution assuming independent encoding
       * Comparison between observed and expected neuronal distributions
       * Statistical analyses using:  
          * Binomial right-tail probabilities
          * Kolmogorov-Smirnov test
          * Geometric mean of binomial probabilities
* **prevalence_simulations.ipnyb:**\
This notebook examine how variable prevalence affects the expected distribution of neuronal encoding under the assumption of independent encoding. It performs analytical and simulation based calculations and generates prevalence related figures.
  * The notebook includes:
      * Calculation of the probability of encoding exactly k variables as a function of prevalence (p₀)
      * Generation of heat maps showing the distribution of encoding probabilities across prevalence values
      * Identification of the prevalence that maximizes the probability of observing neurons encoding a single variable (k=1)
      * Analysis of how the optimal prevalence changes with the number of encoded variables (K)
      * Examination of the asymptotic behavior of specialization probability as K increases

 
## Data 
* **sig_all.mat**:\
contains the binary encoding matrix used for the analyses. Each row represents a single neuron, and the six columns correspond to Cues, Position, Kinematics, Accuracy, Previous reward, and Reward, with entries of 1 or 0 indicating whether the neuron encoded the corresponding variable.

## To run the code 
* Download the notebooks together with the required files:
  * encoding_distribution_analysis.ipynb
  * prevalence_simulations.ipnyb
  * computational_routines.py
  * sig_all.mat
* Place all files in the same folder 
* Open every notebook using Jupyter Notebook
* Run all cells sequentially  
