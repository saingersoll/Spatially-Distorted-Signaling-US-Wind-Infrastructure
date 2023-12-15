# Spatially Distorted Signaling US Wind Infrastructure
The phenomenon of Spatial Distorted Signalling (SDS) describes the mobilization of minority opinion holders to push back electorally. Leah Stokes (et.al) has explored the SDS phenomenon as a natural experiment in her piece, Electoral Backlash against Climate Policy: A Natural Experiment on Retrospective Voting and Local Resistance to Public Policy (2016). The findings in this paper describe that rural Canadian communities had a greater ability to mobilize and organize political pushback against majority chair holders in parliament after the passing of legislation that incentivized the development of wind infrastructure.

Since then, Leah has navigated the nuances of varying percentiles in races, political affiliation (particularly the % precinct gop voting share), the scale and size of the project, as well as, the volume of local mobilization in her research, Replication Data for: Prevalence and predictors of wind energy opposition in North America (2023). 

I am hoping to reproduce these naturally observed outcomes with the US Wind Data and assess the relationship of population density and the project status of wind plants. Analysis of these relationships could provide insight into understanding the scaling effect that local resistance has on spatially distorted signalling in relation to wind infrastructure projects and and sustainable climate policy.

The data source that was utilized in this project, US Wind Data, focuses on the public stance on wind infrastructure for census tract regions within a 3 km buffer zone of a wind plant. It contains categorical variables, binary variables, continuous socioeconomic factors such as % of races, % precinct political gop affiliated voting share, mobilization tactics, and more. Data is associated with the Replication Data for: Prevalence and predictors of wind energy opposition in North America, doi Harvard Dataverse, V1, 2023. The collaborators on that project include: Stokes, Leah; Franzblau, Emma; Lovering, Jessica R.; Miljanich, Chris. Leah Stokes and her awesome team gathered all of this information from American Wind Association (awea), operational, Columbia Sabin Center (columbia).

The SOP covered in this documentation include:
- Defining a binary variable
- Single & Multivariate Logistic Regression Models
- Logit & Log Odds
- Predicitve Probability

Main Takeaways:
Intuitively as expected, a single unit increase in population density is associated with a minor increase in the odds ratio of a wind plant operating. Our models also described that for each single unit increase in median income, there is a decrease in the odds ratio that a wind plant is operational. Similarly, this is seen with anti wind infrastructure opinion holders.

Although our p-values each of our models provided p-values for our coefficients that are hold because they are above the significance level of 0.05. We cannot make any definitive assumptions about our logistic regression models because there is insufficient evidence inspecting the influential effects of omitted variables bias and a lack of data for regions with non-operational wind plants.


Citations:
Stokes, Leah C. “Electoral Backlash against Climate Policy: A Natural Experiment on Retrospective Voting and Local Resistance to Public Policy.” American Journal of Political Science, vol. 60, no. 4, 2016, pp. 958–74. JSTOR, http://www.jstor.org/stable/24877466. Accessed 14 Dec. 2023.

@data{DVN/LE2V0R_2023,
author = {Stokes, Leah and Franzblau, Emma and Lovering, Jessica R. and Miljanich, Chris},
publisher = {Harvard Dataverse},
title = {{Replication Data for: Prevalence and predictors of wind energy opposition in North America}},
year = {2023},
version = {V1},
doi = {10.7910/DVN/LE2V0R},
url = {https://doi.org/10.7910/DVN/LE2V0R}
}
Carleton, Tamma. Eds 222: Week 7: In-Class Lab, 15 Nov. 2023, tcarleton.github.io/EDS-222-stats/labs/07-week-seven/week-7-lab-answers.html. Accessed 14 Dec. 2023. 
If given the opportunity, I would expand the dataset to include any more possible non-operational wind plants and explore in greater detail how exogenous our variables are and determine which values are likely interacting, to produce the best model fit.
