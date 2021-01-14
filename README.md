# Data science project portfolio

A neuroscientist who aspires to become a data scientist!
Thus, it's time to change the lab magic to data magic!
Projects will mostly revolve around my areas of interest, such as healthcare and diseases.
My end goal is to be able help and assist other people in their decision-making with data!

## Table of contents

## Data cleaning & preprocessing
### Monthly updated public COVID-19 dataset from Centers for Disease Control and Prevention
Note! The public dataset is 1.97 GB and could not be downloaded to GitHub. Click the link and you can access the [dataset](https://data.cdc.gov/Case-Surveillance/COVID-19-Case-Surveillance-Public-Use-Data/vbim-akqf)
 

Aim was to clean and preprocess the dataset for use with machine learning and possibly with data visualization.

Public dataset consists of categorical columns created from restricted patient dataset, which resulted in mainly dropping NaN-value rows from the dataset. In the dataset, NaN-values were marked as 'Missing' and additionally, values marked 'Unknown' were present but he data source does not define 'Unknown' values. Before dropping the NaN-values, we converted 'Missing' and 'Unknown' values to NaN.

We created a new column to data set, which shows number of days between first symptoms associated with COVID-19 and first positive test result for COVID-19. Here, it is important to note, that the integer values can be negative or positive. Positive value tells, that the symptoms began before the first positive COVID-19 test result while negative values implicate that patient was tested positive for COVID-19 before first symptoms appeared.

We used Pandas Profiling to take a quick look at the data, and found linear correlations between hosp_yn, icu_yn, death_yn, and weakly with medcond_yn. In case of non-linear correlation age_group is linked to icu_yn, medcon_yn, death_yn, and hosp_yn. Thus, if data is to be used with machine learning, these variables need to be dealt with.
<!--
**katriaksentjeff/katriaksentjeff** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

