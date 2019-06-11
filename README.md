# Electric mobility study

## Summary

This is a study of the electric vehicle market in Europe. The objective is to explain why some countries have a larger market share of  electric cars than others.

I chose a set of characteristics that I suspected correlate with EV market share. These characteristics were:
* Same-sex marriage: allowed or not?
* Gini index (the higher, the greater income inequality)
* Share of votes of nationalist parties
* Social progress index
* GDP per capita (PPP)

I created a predictive model that uses these characteristics as input and predicts the market share of EVs in this (hypothetical) country.

After evaluating multiple models, I settled on a linear regression model that takes into account a subset of these characteristics:

**The resulting model can be viewed [here (interactive)]()**

**Some of the most striking results:**
* Norway is unparalleled in the world when it comes to EV market share. In fact, its numbers were so high that it had to be excluded from model training.
* The time series data on electric car registrations in Europe shows an exponential trend; this is likely to continue in the next years and we should expect the share of EVs to rise immensely
* Nearly every European country sees a steady rise of the market share of EVs; some (Poland, Hungary) more slower than others (Germany, France), but the trend is unmistakable!
* To my surprise, success of nationalist parties does not correlate negatively with EV market share! The other characteristics, however, behave as expected (the strongest correlation is with GDP per capita)

## Notebooks

### Dataset 1 (Data from Eurostat)

* [Data cleaning (Eurostat)](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/notebooks/dataset1-cleaning.ipynb)
* [Dataset creation: EV market share](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/notebooks/dataset1-1-market-share.ipynb)
* [Dataset exploration](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/notebooks/dataset1-exploration.ipynb)

### Dataset 2 (Full data set, model training)

* [Dataset 2: Creation](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/notebooks/dataset2-creation.ipynb)
* [Dataset 2: Exploration](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/notebooks/dataset2-exploration.ipynb)
* [Dataset 2: Model](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/notebooks/dataset2-model.ipynb)
* [Dataset 2: Interactive](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/notebooks/dataset2-interactive.ipynb)

## Data

* [Original data (Eurostat)](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/data/road_eqr_carpda_1_Data.csv)
* [Dataset 1 (cleaned)](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/data/road_eqr_carpda_cleaned.csv)
* [Dataset 2 (cleaned, data for model)](https://nbviewer.jupyter.org/github/maxims94/electric-mobility-study/blob/master/data/dataset2.csv)