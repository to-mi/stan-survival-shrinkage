Bayesian linear survival analysis with shrinkage priors in Stan
===============================================================

Introduction
------------

This repository includes some [Stan][] codes for survival analysis with shrinkage priors (Gaussian, Laplace, and horseshoe) and Weibull observation model. See the reference for the model description (note that the priors on `a_c`, `b_c`, `a_s`, and `b_s` have been changed to half-normal in the codes). The codes have been rewritten for Stan 2.4.0 (reference used Stan 2.2).

  [Stan]: http://mc-stan.org/

Contents
--------

 * `example.R`: R-script which generates some simulated data and fits the models.
 * `wei_hs_joint.stan`: Joint model with horseshoe prior on candidate biomarkers.
 * `wei_lap_joint.stan`: Joint model with Laplace prior on candidate biomarkers.
 * `wei_gau_joint.stan`: Joint model with Gaussian prior on candidate biomarkers.
 * `wei_bg_joint.stan`: Joint model with only established risk factors.
 * `wei_hs.stan`: Single-group model with horseshoe prior on candidate biomarkers.
 * `wei_lap.stan`: Single-group model with Laplace prior on candidate biomarkers.
 * `wei_gau.stan`: Single-group model with Gaussian prior on candidate biomarkers.
 * `wei_bg.stan`: Single-group model with only established risk factors.

Reference
---------

Peltola, Havulinna, Salomaa, Vehtari. _Hierarchical Bayesian Survival Analysis and Projective Covariate Selection in Cardiovascular Event Risk Prediction._ In Proceedings of the Eleventh UAI Bayesian Modeling Applications Workshop, CEUR Workshop Proceedings, Vol-1218, 79-88 ([pdf][])

  [pdf]: http://ceur-ws.org/Vol-1218/bmaw2014_paper_8.pdf

Contact
-------

E-mail: tomi.peltola@aalto.fi
