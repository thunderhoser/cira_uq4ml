# Uncertainty quantification for machine learning at Cooperative Institute for Research in the Atmosphere

This repository is a companion to the following journal paper:

Haynes, K., R. Lagerquist, M. McGraw, K. Musgrave, and I. Ebert-Uphoff, 2022: "Creating and evaluating uncertainty estimates with neural networks for environmental-science applications." *Artificial Intelligence for the Earth Systems*, **under review**.

This repository contains several Jupyter notebooks for implementing the methods discussed in the paper -- both the UQ methods themselves and the evaluation methods for uncertainty estimates.

 - `mc_dropout_for_classification.ipynb` implements MC dropout for digit classification.
 - `quantile_regression_for_classification.ipynb` implements quantile regression for digit classification, using a special NN architecture that prevents quantile-crossing.  Both notebooks use the spread-skill plot and discard test to evaluate uncertainty estimates.
 - `crps_loss.ipynb` implements the continuous ranked probability score (CRPS) as a loss function.
 - `uq_regression.ipynb` implements three UQ methods (parametric prediction, CRPS loss function, and MC dropout) for six synthetic datasets and uses four methods to evaluate the models (spread-skill plot, discard test, PIT histogram, and reliability curve).
