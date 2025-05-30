## Spatially Distorted Signaling: How Opinions Against Wind Infrastructure Delay Our Transition to Renewable Energy

### 🗃️Blog Post: [https://github.com/saingersoll/Spatially-Distorted-Signaling-US-Wind-Infrastructure](https://saingersoll.github.io/posts/2023-12-14_SDS_Wind_Infrastructure/SDS_Wind_Infrastructure.html)

### Overview

Spatial Distorted Signalling (SDS) is a term that describes the mobilization of minority opinion holders to electorally push-back and promote legislation that aligns with their beliefs (Stokes, et al, 2016). The SDS phenomenon has the ability to skew the accurate representation of public opinions due to effective organization practices. This leads to a disproportionate number of minority opinion holder interactions spent influencing local legislators and collective voting in smaller elections. Natural occurrences of the SDS phenomenon were recently observed in rural Canadian communities after new legislation was passed by the Green Party to incentivize large-scale wind power developments. Minority opinion holders gathered strategically to vote out the Green Party in the following election in retaliation and succeded. The policy was amended shortly after, halting new production of wind power infrastructure. Within the U.S. a number of wind plant developments have encountered similar outcomes. In this investigation, we will seek to understand how population density, median income, and anti-wind power opinions impacted wind plant operational activity (2000-2016), providing insights into local resistance and its effects on renewable energy projects.

![image](https://github.com/user-attachments/assets/2a6f6d06-4074-48c8-bd7b-7f83160059d7)
Figure: Wind turbines on the Bishop Hill wind farm operate among the corn and soybean fields near Bishop Hill, Illinois (U.S. Department of Agriculture, 2017).

### `Main Takeaways`

The overarching logit model analysis did not provide significant findings, but alluded to influential covariate interactions. The multivariate interaction model was leveraged to tabulate individually significant propensities. The probabilities revealed increased median income appeared to inhibit the forward progression in clean energy developments. Further exploration of the covariate interactions are encouraged with expanded datasets, as a limited amount of data was utilized for this study, restricting the sample analysis. Using what is currently available, we will interpret the socioeconomic factors in this model as they relate to real-world social and political dynamics.
Population Density

#### `Population Density`
Interestingly, pro/neutral-wind power areas demonstrated an increase in population density and median income was associated with a decrease in the odds of having an operational wind power plant. It was revealed in areas with pro/neutral-wind power sentiments with the lowest income percentile were an exception and experienced an increase in the odds of an active wind plant as population density increased. Whereas in anti-wind regions, as population density increased an inverse effect was observed. Across all median income groups, anti-wind areas with higher population densities had marginally greater odds of having an active wind plant. These anti-wind findings suggested areas with lower population density are at greater risk of experiencing SDS. Both trends revealed could be an indication of the magnitude in which socioeconomic interactions influence sustainable energy developments.

#### `Median Income`
Overall, higher-income areas were found to have increased odds of deactivated wind plants. Regardless of a pro/neutral-wind power sentiment, as the median wealth increased the odds of operational activity decreased. This may be an indicator that wealthier areas are at greater risk of experiencing SDS due to disproportionate access to financial resources that influence energy policy decisions. Advantages such as wealth assist minority opinion holders when strategically lobbying to tailor policies to better align with their priorities. Uneven socioeconomic power-dynamics lead to minority opinion holders preventing the development of wind power infrastructure, alongside other renewable energy solutions. Overall, these findings suggest that socioeconomic factors play a heavily influential role in shaping renewable energy projects.

#### `Anti-Wind Infrastructure Opinion`
As suspected, areas with higher opposition to wind infrastructure were less likely to have operational wind plants. Conversely, the opposite was seen for pro/neutral-wind opinion holding areas. This aligns with expectations that local opposition and social mobilization impacts the establishment of wind plants. Therefore, addressing and mitigating local resistance is essential for enhancing the feasibility and acceptance of wind energy initiatives.

### U.S. Wind Power Plant Data

- [Replication Data for: Prevalence and predictors of wind energy opposition in North America](https://dataverse.harvard.edu/file.xhtml?fileId=7339850&version=1.0)

The data source that was utilized in this project, US Wind Data, focuses on the public stance on wind infrastructure for census tract regions within a 3 km buffer zone of a wind infrastructure project. It contains categorical variables, binary variables, continuous socioeconomic factors such as % of races, % precinct political gop affiliated voting share, mobilization tactics, and more. This data is associated with the Replication Data for: Prevalence and predictors of wind energy opposition in North America, doi Harvard Dataverse, V1, 2023. The collaborators on that project include: Stokes, Leah; Franzblau, Emma; Lovering, Jessica R.; Miljanich, Chris. Leah Stokes and her awesome team gathered all of this information from American Wind Association ("awea"), operational, Columbia Sabin Center ("Columbia").

### Techniques Applied
- Single & Multivariate Logit Regression Models

- Logit Model & Log Odds

- Predicted Probability & P-test

### Limitations
#### `Insufficient Data & Omitted Variable Bias (OVB) & Ethical Critiques`
It is important to note that there was heavy bias towards operational wind plants within the dataset, as observed in the data distribution visualization and in Summary Coefficients Table (Figure 1, Table 1). The table described a baseline 60% odds ratio of having an operational wind plant. The overall model did not provide significant findings, but encouraged deeper exploration of the data. When interpreting the model on a more granular level, the p-values across all combinations of the pro/neutral-wind percentile probabilities were found to be highly significant (**p < 0.001), and roughly half of the anti-wind probabilities were found to be significant (**p < 0.05). Although the propensity scores illuminated some trends relating higher median income and lower wind plant operational activity, these results are not statistically bolstered enough to use as strong conclusions. 

The data set may lack comprehensive factors affecting wind plant activity, such as specific local policies or environmental conditions. The analysis is limited by omitted variables which may be additionally influence wind plant activity. Ensuring the exogeneity of variables is challenging, and logistic regression models do not account for all underlying factors. This is not an appropriate analysis to use for definitive decision making, rather it is an introspection on influencing socioeconomic dyanmics at hand. It is not a complete representation of the populous and requires additional data to support trends discussed in the paper. The lack of significance across the board suggests there may be insufficient evidence to definitively assess the impact of these variables on wind plant activity. This interpretation is intended to be used as starting point for deeper analysis. 


### Data Citation
```
1. Stokes, Leah; Franzblau, Emma; Lovering, Jessica R.; Miljanich, Chris. "Replication Data for: Prevalence and predictors of wind energy opposition in North America", https://doi.org/10.7910/DVN/LE2V0R, Harvard Dataverse, V1, 2023.
```
![image](https://github.com/user-attachments/assets/306e9255-2892-4fee-bf61-20c176bc1cfd)

