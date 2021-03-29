Overall Impression
==================

Summary of Report
-----------------

A driver’s ability depends on the perception,
alertness, awareness, and response time of the driver. Alcohol is known
to impair all those qualities, and therefore has a negative effect on
driving. The data for this project was taken from a population-based
study by the National Highway Traffic Safety Administration’s Fatal
Accident Reporting System (FARS) across 48 states from 1982 to 1988.
Hawaii, Alaska, and the District of Columbia were not included in the
study. The objective of this project is to build a predictive model
using alcohol related variables to estimate the percent of total
fatalities (alcoholic fatalities/total fatalities). The variables that
were chosen were mandatory jail sentence, mandatory community service,
tax on case of beer, minimum drinking age, percent residing in dry
counties, unemployment, spirits consumption, and preliminary breath test
law. The exploratory data analysis indicated that all variables except
percentage of dry counties and the percentage of alcoholic fatalities
had a decreasing trend per unit increase in year. A fixed effect model
from panel regression analysis was deemed the best model after
appropriate tests (Breusch-Pagan LM test and Pesaran CD test) were run.
It was found that spirits consumption, mandatory jail sentence, and
mandatory community service were significant. The model showed cross
sectional dependence indicating a lack of independence between states
for the outcome variable. The model’s implications are that state and
local governments need to create and enforce stricter laws on drunk
driving particularly pertaining to spirits consumption and mandatory
jail sentence. 

Overall Impression
------------------

The report defined the question of interest
clearly and provided background information and impact of the question
of concern. The authors put much effort in providing good data
visualization which helped readers to better understand the variables in
the dataset, especially the change in certain variables overtime.
However, the exploratory data analysis plots seemed to take up too much
space in the report and can be more succinct. For inferential analysis,
the model selection process was well explained and justified, but model
outcomes should be presented more clearly. It was suggested to use
propensity score to facilitate causal interpretation.

Major Comments
==============

1. For the introduction section, it was
suggested to provide a general overview of the variables included in the
model. Introduction to dataset and variables was covered in the
background section of the report, and the introduction section mainly
provided information on the question of interest, the significance of
the question, objective of the report, as well its impact. No details of
the dataset was included in the introduction. The authors decided to
keep the way the materials were organized in the report because it is
clear to have a separate introduction and background section focusing on
different aspects of the project. Also, it makes sense to first have an
overview of the problem in the introduction, and then go to specific
dataset and variables in the later background section. 

2. The background section is one long
paragraph. It will be helpful to break it down into several sub-sections
and give each sub-section a heading, such as dataset, variables, etc.
This would give readers a clearer structure of the material. 

3. The comments towards the descriptive
analysis section were generally positive. In particular, the Exploratory
Data Analysis (EDA) section at 4.2 gave readers a good idea of the
distribution of the data, even if they had no prior understanding of the
data. For example, the first bar chart in 4.2.1.1 is able to convey the
message that certain states had significantly higher spirits consumption
than any other state in the US. Readers generally enjoyed the
interactive plots such as the US Traffic Fatalities map in Section 4.1
as it gives them a good idea of how the different metrics used to
understand the alcohol related fatalities can actually bring different
results. One of the other issues of the analysis was that the response
variable was the proportion of alcohol fatalities (alcoholic
fatalities/total fatalities). The goal of the project was to determine
factors that lead to an increase or decrease in fatalities. The
proportion of alcoholic fatalities does not measure a decrease because a
decrease in alcoholic fatalities will affect the total fatalities
keeping the proportion constant. To fix this the response variable
should be changed to a standardized rate of alcoholic fatalities.


4. There was some constructive feedback in
this section. One of the feedback was the distraction caused by the
large number of visualizations. In other words, certain plots that
aren’t significant in helping the readers understand the data, or plots
that look messy in general can be eliminated. Some examples are the bar
chart on dry resident proportions and the histogram on the number of
fatalities. The former does not help readers understand how the dry
resident proportions can potentially affect the number of alcohol
related fatalities, while the latter isn’t of much use since the number
of fatalities was not directly used in the model selection and analysis
anyway. Another plot that wasn’t really well received is the line plot
of the proportion of alcohol related fatalities of each state against
the year (Section 4.2.1.2) as it looked too messy. Other than removing
this plot, another thing that can be done to improve the situation is to
only include that lines of states with extraordinary trends, eg.
Mississippi (MS) and North Dakota (ND) .

4. There was some constructive feedback in
this section. One of the feedback was the distraction caused by the
large number of visualizations. In other words, certain plots that
aren’t significant in helping the readers understand the data, or plots
that look messy in general can be eliminated. Some examples are the bar
chart on dry resident proportions and the histogram on the number of
fatalities. The former does not help readers understand how the dry
resident proportions can potentially affect the number of alcohol
related fatalities, while the latter isn’t of much use since the number
of fatalities was not directly used in the model selection and analysis
anyway. Another plot that wasn’t really well received is the line plot
of the proportion of alcohol related fatalities of each state against
the year (Section 4.2.1.2) as it looked too messy. Other than removing
this plot, another thing that can be done to improve the situation is to
only include that lines of states with extraordinary trends, eg.
Mississippi (MS) and North Dakota (ND) .

5. The inferential analysis section gave a
good explanation of the model. The assumptions of the model and why the
model was chosen were well described and justified. There was some
missing information on the model outcome, for example the fitted values
results (point estimation, 95% CI, P-value). It will be easier for
readers to find crucial information if they can be compiled in a table.


6. Hypothesis testing whether predictors of
interest(breath, jail, service) are significantly different from zero or
not should be explicitly stated and interpreted as it helps quantify
what we discovered.

7. Another Issue was that the causal
interpretation was missing the propensity score which is the probability
of a unit being assigned to a particular treatment. This type of
analysis would give a numerical score to the causal interpretation which
would make it clearer why causal interpretation cannot be made. 

8. Besides explaining how the final model was
chosen and comparing all the models that have been considered,, more
emphasis should be put on analyzing the effect of predictors included in
the model and interpreting such results. The null hypothesis and test
statistic for testing each effect of interest should be explicitly laid
out, together with the outcomes.

Minor Comments
==============

1. A minor issue that was raised in regards
to the visualizations in the descriptive analysis section is
consistency. Particularly, some plots did not contain titles (eg. 2nd
set of bar charts in 4.2.1.1 and the boxplots in 4.2.2) and some plots
have missing axis labels (the 2nd last set of plots before Section 5).
More attention should be paid in this regard to make those
visualizations clear and understandable.

2. The spacing between text and plots should
be adjusted and kept constant.

 3. Some sections of the report are
figure-heavy (e.g. data description), while others are text-heavy
(background, causal interpretation, and discussion). Figures can
alternate with texts for a better reading experience.
