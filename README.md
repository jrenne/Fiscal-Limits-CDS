# FISCAL LIMITS AND SOVEREIGN CREDIT SPREADS
# Kevin PALLARA and Jean-Paul RENNE
# This version: May 2020.


These codes replicate the results of the paper entitled “Fiscal limits and sovereign credit spreads”, by Kevin Pallara and Jean-Paul Renne, see https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3475425


A- How to run the codes?

The script “main.R” makes it possible to run the estimation and, further, to produce the paper’s charts as well as the table of parameter estimates.

Before sourcing “main.R”, modify the working directory (line 12 of main.R).

In main, you can, in particular:
- select the countries to consider (“list.of.ctries”),
- determine whether the estimation (maximisation of the likelihood) is run (“indic.estim”  set to 1 (Yes) or 0 (No)),
- define how to operate the estimation — in particular, set “indic.use.parallel” to 1 if you want to use parallel computing (the country-specific estimations will be carried out by different cores); in this case, specify the number of cores to use (“number.of.cores”),
- set some constraints on estimated parameters,
- the number of rows on plots in figures, and whether figures include colours or not.


B- Organisation of codes

The folders are as follows:

- “estimation” contains codes allowing for the estimation of the models.
- “procedures” contains various procedures, organised in different scripts according to their use.
- “data” contains the data used by the estimation (see next section).
- “results” contains R data files with the specification of previously saved models.
- “load.data.files” contains scripts that load and organise the data. 
- “outputs” contains output charts and tables, as well as the scripts producing these output files.


C- Data

The data are gathered in the “data” folder. There is one folder per country. Each country folder contains a specific readme file detailing the sources of the data. These folders notably contain Excel files that allow for the extraction of Datastream data.

