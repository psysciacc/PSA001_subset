# PSA001subset

This project contains 1/3 of the raw and processed data (the **exploratory segment**) for PSA001 (social faces), which we are releasing for the [Secondary Analysis Challenge](https://psysciacc.org/2019/09/01/introducing-the-psa001-secondary-analysis-challenge/).

Click on the badge below to open the files in a binder container.

  <!-- badges: start -->
  [![Launch Rstudio Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/psysciacc/PSA001subset/master?urlpath=rstudio)
  <!-- badges: end -->


### PSA001 project: To Which World Regions Does the Valence-Dominance Model of Social Perception Apply?

Over the last ten years, Oosterhof and Todorov’s valence-dominance model has emerged as the most prominent account of how people evaluate faces on social dimensions. In this model, two dimensions (valence and dominance) underpin social judgments of faces. To which world regions this model applies is a critical, yet unanswered, question. We address this question by replicating Oosterhof and Todorov’s methodology across multiple world regions. 

This repository contains the following files:

#### Code 

* `psa001_RR_subset.html`: Documentation of the primary analyses used in this project. Start here if you want to know what analyses the PSA001 project team will be reporting in their Registered Report.
* `psa001_RR_subset.Rmd`: The R file used to generate `psa001_RR_subset.html`

#### Raw data

We stratified by lab before sampling the exploratory segment -- in other words, the data are a randomly-sampled 1/3 of each lab's data

* `data/psa001_exp_data_subset.csv`: Data from the rating experiments
* `data/psa001_quest_data_subset.csv`: Data from the demographic questionnaires
* `data/psa001_session_subset.csv`: Session data containing information about lab, language, and trait rated

#### Processed data

Processed data files are created by the script, but also provided here. Each has an associated codebook.

* `data/psa001_ratings_raw_subset.csv`: The joined version of the three raw exploratory datasets (i.e., pre-aggregation)
* `data/psa001_ind_subset.csv`: The processed version of the exploratory dataset, with one row for each subject/stimulus/rating. 
* `data/psa001_agg_subset.csv`: The processed version of the exploratory dataset, aggregated with one row for each region/stimulus/rating

#### Auxillary files

* `Karolinska_14trait_judgmentswithlabels.xls`: Ratings from Oosterhof & Todorov (2008)
* `Karolinska_ReadMe_Updated2012.txt`: Documentation on the factor loadings from Oosterhof & Todorov
* `regions.csv`: A look-up table that translates the region codes used in the raw and processed datasets into the larger regions used for the paper
* `alphas.RDS`: A file (readable by R) that contains Cronbach's alphas. This file can be loaded into R to produce figures/tables instead of calculating the Cronbach's alphas in the R session (which takes some time)


## Resources

* [PSA001 OSF Project](https://osf.io/f7v3n/)
* [Preprint of Registered Report](https://psyarxiv.com/n26dy) (Accepted in principle at Nature Human Behaviour)
* [PSA001 Social Faces Data Management Plan.docx](https://osf.io/v46q8/)
* [Psychological Science Accelerator: PSA001](https://psysciacc.org/001-face-perception/)
* [Try the study in any language](https://psa.psy.gla.ac.uk/)



