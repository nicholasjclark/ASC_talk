# ASC talk on time series analysis / forecasting with {mvgam}
## Abstract
Time series analysis and probabilistic forecasting are standard goals in applied statistics. But most time series tools available to applied researchers are restricted to traditional forecasting models such as ARIMA, GARCH or Exponential Smoothing variants. These models cannot readily handle features that dominate many real-world datasets (particularly those in ecology), including overdispersion, clustering, missingness, discreteness and nonlinear effects. Using the flexible and powerful probabilistic programming ecosystem Stan, we can build more appropriate time series models to meet this complexity head on. In this talk I will introduce Bayesian Dynamic Generalized Additive Models (DGAMs) and illustrate their advantages for analyzing and forecasting real-world time series. I will discuss [{mvgam}](https://nicholasjclark.github.io/mvgam/), an open-source R package that can fit DGAMs with nonlinear effects, hierarchical effects and dynamic processes to data from a wide variety of observation distributions. These models are especially useful for analysing multiple series, as they can estimate hierarchical smooth functions while learning complex temporal associations with latent vector autoregressive processes or dimension-reduced dynamic factor processes. Because the package uses Hamiltonian Monte Carlo inference through Stan, it is straightforward to create Stan code and all necessary data structures so that additional stochastic elements can be added to suit the user's bespoke needs. Other key features of {mvgam} are functions to critique models using rolling window forecasts and posterior predictive checks, online data augmentation via a recursive particle filter and graphical tools to visualise probabilistic uncertainties for smooth functions and predictions. I hope to show how models that describe real-world complexity, both through nonlinear covariate functions and multi-series dependence, are useful to ask targeted questions about drivers of change.

## Bio
Dr. Nicholas Clark is an Australian Research Council Early Career Fellow in the [School of Veterinary Science at the University of Queensland](https://researchers.uq.edu.au/researcher/15140). He is broadly interested in exploring new ways to (1) understand how ecological communities are formed and (2) predict how they will change over time. Dr Clark’s research focuses on developing computational tools and adapting techniques from statistical forecasting to study how organisms and ecosystems respond to change, with applications across a variety of ecological systems. He is also the developer of {mvgam}, an R package for fitting and interrogating Bayesian Dynamic GAMs.

## Slides
The slidedeck can be [accessed as an html version](https://nicholasjclark.github.io/ASC_talk/ASC_talk_slidedeck#1)
