# Uncertainty quantification for machine learning at Cooperative Institute for Research in the Atmosphere

This repository is a companion to the following journal paper:

Ebert-Uphoff, I., R. Lagerquist, K. Haynes, M. McGraw, and K. Musgrave, 2022: "Methods to evaluate uncertainty estimates provided by neural networks in environmental science applications." *Artificial Intelligence for the Earth Systems*, **under review**.

[Colab notebook for quantile regression](https://colab.research.google.com/drive/1qB9LfEOe8ZBaXdyw4pL-6Hs6ptIjXEGC)
<br />
[Colab notebook for Monte Carlo dropout](https://colab.research.google.com/drive/1h_lmmD98fv7pmIAXsdA433bWKQOEw42O)

Notes from Ryan to all:
 - I wonder if there's a way to include Colab notebooks directly in the Github repo, instead of just linking to them in the README.  I like Colab *much* better than Jupyter, but it would be nice if there were a more elegant way to include the notebooks in Github.  Also, this would give us a way to create a release that accompanies the paper, where the code is frozen.  Then we can edit the notebooks in the future without worrying.
 - I mostly like my notebook for quantile regression, except I need to add some figures (*i.e.*, plot digit examples with low uncertainty and some with high uncertainty).  The notebook for MC dropout contains no explanatory text right now, so I need to add that, then add similar figures to the MC-dropout notebook as for the QR notebook.
