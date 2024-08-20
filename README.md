## Spatially Distorted Signaling: How Opinions Against Wind Infrastructure Delay Our Transition to Renewable Energy

### 🗃️Blog Post: [https://github.com/saingersoll/Spatially-Distorted-Signaling-US-Wind-Infrastructure](https://saingersoll.github.io/posts/2023-12-14_SDS_Wind_Infrastructure/SDS_Wind_Infrastructure.html)

### Main Takeaways

- **Population Density**: Effect: A unit increase in population density is associated with a slight increase in the odds of having an operational wind plant. This suggests that areas with higher population densities are marginally more likely to host wind plants and less likely to experience minority holder opinions taking the majority.

- **Median Income**: Effect: An increase in median income is linked to a decrease in the odds of having an operational wind plant. Higher income areas show a lower likelihood of wind plant activity, potentially due to different local priorities or economic factors. Uneven socio-economic power-dynamics could lead to minority opinion holders preventing the development of wind power infrastructure, alongside other renewable energy solutions.

- **Anti-Wind Infrastructure Opinion**: Effect: Areas with higher opposition to wind infrastructure are less likely to have operational wind plants. This aligns with expectations that local opposition impacts the establishment of wind plants.
![image](https://github.com/user-attachments/assets/2ff1a5fe-d0e3-4721-ad2c-836e7e238446)
The world's largest wind turbine, MySE-16-260. Includes a rotor diameter of 853 feet to produce 16-megawatt, located in Pingtan, Fujian Province, China (Yang, Getty Images).

### Overview

This study aims to visualize the activity of U.S. wind power plants (2000-2016) to understand how population density, income, and anti-wind opinions impact wind plant activity. Spatial Distorted Signalling (SDS) describes the mobilization of minority opinion holders electoral push-back to promote legislation that aligns with their beliefs. The motivation for this project is to provide insights into attributes that contribute to local resistance and their effects on renewable energy development.

### Background 
Leah Stokes (et.al) has explored the SDS phenomenon as a natural experiment in her piece, Electoral Backlash against Climate Policy: A Natural Experiment on Retrospective Voting and Local Resistance to Public Policy (2016). The findings in this paper describe that rural Canadian communities had a greater ability to mobilize and organize political push back against majority chair holders in parliament after the passing of legislation which invited the development of wind infrastructure through incentives. Since then, Leah has navigated the nuances of varying percentiles in races, political affiliation (particularly the % precinct gop voting share), the scale and size of the project, as well as, the volume of local mobilization in her research, Replication Data for: Prevalence and predictors of wind energy opposition in North America (2023). 

This project explores US Wind Data to observe wind plant activity stauts and assess the effect of population density, median income ($), and anti-wind opinion on wind plants. Analysis of these relationships could provide insight into understanding the scaling effect that local resistance has on spatially distorted signalling in relation to wind infrastructure projects and and sustainable climate policy.

### Techniques Applied

- Single & Multivariate Logit Regression Models

- Logit & Log Odds

- Predictive Probability

- Ethical Critiques & Addressing Limitations

### Limitations

##### `Considering Omitted Variable Bias (OVB)`

Neglecting additional variables without testing is improper practice. Exogeneity is a very difficult OLS assumption to uphold – alongside a normal distribution of the error mean. A means to determine relationships between variables is running various linear regression models and comparing the $R^2$ value. In this project, we focus our attention on the why OLS was not the analysis method of choice for our relationships of interest. In the instance of logistic regression, a log odds ratio must be taken to interpret each individual variable. There is a strong possibility that the models utilized in this project are not exogenous and require deeper analysis to determine the impact of underlining influences.

##### `Insufficient Data`

The data set may not fully capture all relevant factors affecting wind plant activity, such as specific local policies or environmental conditions.

### `U.S. Wind Power Plant Data`

- [Replication Data for: Prevalence and predictors of wind energy opposition in North America](https://dataverse.harvard.edu/file.xhtml?fileId=7339850&version=1.0)

The data source that was utilized in this project, US Wind Data, focuses on the public stance on wind infrastructure for census tract regions within a 3 km buffer zone of a wind infrastructure project. It contains categorical variables, binary variables, continuous socioeconomic factors such as % of races, % precinct political gop affiliated voting share, mobilization tactics, and more. This data is associated with the Replication Data for: Prevalence and predictors of wind energy opposition in North America, doi Harvard Dataverse, V1, 2023. The collaborators on that project include: Stokes, Leah; Franzblau, Emma; Lovering, Jessica R.; Miljanich, Chris. Leah Stokes and her awesome team gathered all of this information from American Wind Association ("awea"), operational, Columbia Sabin Center ("Columbia").

### Data Citation

{1. Stokes, Leah; Franzblau, Emma; Lovering, Jessica R.; Miljanich, Chris. "Replication Data for: Prevalence and predictors of wind energy opposition in North America", https://doi.org/10.7910/DVN/LE2V0R, Harvard Dataverse, V1, 2023.}

![image](https://github.com/user-attachments/assets/306e9255-2892-4fee-bf61-20c176bc1cfd)

