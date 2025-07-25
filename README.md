# An Analysis of Misspecification in Nonparametric Estimation of an Autoregressive Process

This repository contains the notebook and the internship report of a research project conducted as part of an internship within the **SAMOVAR laboratory at Institut Polytechnique de Paris**, under the supervision of Professor **Stefano Fortunati**.

The project focuses on the impact of **model misspecification** in time series analysis, particularly in **first-order autoregressive processes (AR(1))**, when classical assumptions—such as Gaussian noise—are violated. This work highlights the limitations of classical statistical tools such as the **Cramér-Rao Bound (CRB)** under model mismatch and emphasizes the benefits of robust estimation techniques.

The theoretical foundations of this work are based on:

- Fortunati, Gini, Greco, and Richmond (2017): *"Performance Bounds for Parameter Estimation under Misspecified Models"*, IEEE Signal Processing Magazine.
- J. Allal, A. Kaaouach, and D. Paindaveine (2001), “R-estimation for arma models,” Journal of Nonparametric Statistics, vol. 13, no. 6, pp. 815–831


## Key Contributions and Findings

- **Misspecified Cramér-Rao Bound (MCRB):**  
  We derive and analyze the MCRB for AR(1) processes with t-distributed noise.

- **Estimator Comparison (MLE, Newton, M- and R-estimators):**  
  The project compares various estimation methods:
  - Maximum Likelihood Estimators (MLE) for Gaussian and Student-t models,
  - Newton-based approximations of the MLE,
  - M-estimators using Huber and Tukey loss functions,
  - R-estimators based on rank statistics.

- **Simulation-Based Analysis:**  
  Extensive Monte Carlo simulations are conducted to compare the Mean Squared Error (MSE) of each estimator under varying degrees of freedom (ν), sample sizes (N), and AR parameters (θ). The results clearly illustrate the advantage of robust estimators under model misspecification.

- **Asymptotic Analysis of R-estimators:**  
  We study the asymptotic properties of R-estimators and propose a corrected version based on known constants, showing that R-estimators can achieve performance close to or better than M-estimators when properly implemented.

## Repository Contents

- `misspecified statistics and autoregressives processes.ipynb`:  
  A Jupyter Notebook implementing all estimation methods, CRB/MCRB derivations, and simulation experiments.

- `misspecified statistics and autoregressives processes report.pdf`:  
  A detailed internship report summarizing theoretical developments, estimator properties, and empirical results.

## Conclusion

This project highlights the importance of robust statistical tools for parameter estimation in autoregressive models, especially in non-Gaussian settings. It emphasizes that assuming a well-specified model can lead to underestimated uncertainties and degraded estimator performance, and demonstrates how modern robust techniques can mitigate these issues effectively.
