# Effect of alcohol regulation and drunk driving laws on alcohol-involved traffic fatalities ratio in 1982-1988

Authors: Yixing Lu, Apurv Srivastav, Liela Meng, Zeng Fung Liew

---
**Project Description** <br>
The objective of this project is to build a predictive model that uses the variables: mandatory jail sentence, mandatory community service, tax on case of beer, minimum drinking age, percent residing in dry counties, unemployment, spirits consumption, and preliminary breath test law to estimate the percent of alcoholic fatalities (alcoholic fatalities/total fatalities). The data for this project comes from the National Highway Traffic Safety Administration’s Fatal Accident Reporting System (FARS), which can be accessed via the [`AER` package](https://rdrr.io/cran/AER/man/Fatalities.html) in `R`.

Panel regression analysis using the fixed effect model was found to be the most appropriate in predicting percent of alcoholic fatalities with significance found for spirits consumption, mandatory jail sentence, and mandatory community service. However, the model also showed cross sectional dependence indicating a lack of independence between states for the outcome variable.  The findings indicate that state and local governments need to create and enforce stricter laws on drunk driving.

## Note
Markdown versions of our HTML reports have been added, but interactive plots in the HTML reports are only available as snapshots. For the full interactive experience with those plots, please download and view the HTML reports on a web browser.
