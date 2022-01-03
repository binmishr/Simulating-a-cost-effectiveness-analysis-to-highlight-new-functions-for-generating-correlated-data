# Simulating-a-cost-effectiveness-analysis-to-highlight-new-functions-for-generating-correlated-data

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same.

A Brief Introduction
======================

The simstudy package is a collection of functions that allow users to generate simulated data sets in order to explore modeling techniques or better understand data generating processes. The user defines the distributions of individual variables, specifies relationships between covariates and outcomes, and generates data based on these specifications. The final data sets can represent randomized control trials, repeated measure designs, cluster randomized trials, or naturally observed data processes. Other complexities that can be added include survival data, correlated data, factorial study designs, step wedge designs, and missing data processes.

Simulation using simstudy has two fundamental steps. The user (1) defines the data elements of a data set and (2) generates the data based on these definitions. Additional functionality exists to simulate observed or randomized treatment assignment/exposures, to create longitudinal/panel data, to create multi-level/hierarchical data, to create datasets with correlated variables based on a specified covariance structure, to merge datasets, to create data sets with missing data, and to create non-linear relationships with underlying spline curves.

The overarching philosophy of simstudy is to create data generating processes that mimic the typical models used to fit those types of data. So, the parameterization of some of the data generating processes may not follow the standard parameterizations for the specific distributions. For example, in simstudy gamma-distributed data are generated based on the specification of a mean μ (or log(μ)) and a dispersion (d), rather than shape α and rate β parameters that more typically characterize the gamma distribution. When we estimate the parameters, we are modeling μ (or some function of μ), so we should explicitly recover the simstudy parameters used to generate the model, thus illuminating the relationship between the underlying data generating processes and the models.
