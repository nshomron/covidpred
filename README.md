## Machine learning-based prediction of COVID-19 diagnosis based on symptoms
[npj Digital Medicine](https://www.nature.com/articles/s41746-020-00372-6) | [medRxiv](https://www.medrxiv.org/content/10.1101/2020.05.07.20093948v2) | [PDF](https://www.nature.com/articles/s41746-020-00372-6.pdf)

[Yazeed Zoabi](https://yazeedzoabi.com)<sup>1</sup>, [Shira Deri-Rozov](https://nshomron.github.io/)<sup>1</sup>, [Noam Shomron](https://nshomron.github.io/)<sup>1</sup><br />
<sup>1</sup> Tel Aviv University

*This framework can be used, among other considerations, to prioritize testing for COVID-19 when testing resources are limited.*

## Model Predictors and Exact Variable Names (True = 1, False = 0)
* **Age over 60** - Age_60
* **Sex** - Male (Male=1, Female=0)
* **Cough** - Cough
* **Shortness of breath** - Shortness_of_breath
* **Fever** - Fever
* **Sore throat** - Sore_throat
* **Headache** - Headache
* **Contact with a confirmed individual** - Contact_with_confirmed



## Model Outcome
The probability of being diagnosed with a COVID-19 infection.


## Use
1. Import lgbm_model_*.txt using LightGBM 2.3.1 on Python 3.6.

2. Predict using your data.

## Files in this repository

* **lgbm_model_all_features.txt** - The predictor that uses all 8 features
* **lgbm_model_balanced_features.txt** - The predictor that uses only balanced symptoms
* **hyperparameters.txt** - The hyperparameters used by lightGBM
* **data/corona_tested_individuals_ver_0083.english.csv.zip** - The tested individuals dataset downloaded from https://data.gov.il/dataset/covid-19 on November 15, 2020 and translated into English
* **data/corona_tested_individuals_ver_006.english.csv.zip** - The tested individuals dataset downloaded from https://data.gov.il/dataset/covid-19 on May 4, 2020 and translated into English. This is the version we used for the analysis.

