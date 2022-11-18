# Uncertainty quantification for machine learning at Cooperative Institute for Research in the Atmosphere

This repository is a companion to the following journal paper:

Haynes, K., R. Lagerquist, M. McGraw, K. Musgrave, and I. Ebert-Uphoff, 2022: "Creating and evaluating uncertainty estimates with neural networks for environmental-science applications." *Artificial Intelligence for the Earth Systems*, **under review**.

This repository contains several Jupyter notebooks for implementing the methods discussed in the paper -- both the UQ methods themselves and the evaluation methods for uncertainty estimates.

 - `classification_mc_dropout.ipynb` implements MC dropout for digit classification.
 - `classification_npdp.ipynb` implements quantile regression for digit classification, using a special NN architecture that prevents quantile-crossing.  Both notebooks use the spread-skill plot and discard test to evaluate uncertainty estimates.
 - `crps_loss.ipynb` implements the continuous ranked probability score (CRPS) as a loss function for ensemble prediction (EP).
 - `regression_multi_datasets.ipynb` allows the user to select one UQ approach (PDP, EP, or MC dropout), then compares the results across seven synthetic datasets.  It uses four evaluation graphics (the attributes diagram, spread-skill plot, discard test, and PIT histogram) and eight evaluation scores (MSESS, SSRAT, SSREL, MF, DI, PITD, CRPS, and IGN).
 - `regression_multi_model.ipynb` allows the user to select one synthetic dataset, then compares the results across the three UQ approaches, using the same evaluation tools.
