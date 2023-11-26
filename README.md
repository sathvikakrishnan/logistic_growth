# Logistic Growth

Here are the R scripts for a reproducible analysis of logistic growth using "experiment2.csv" 🔗 : 

*Question 1*

When fitting a linear model, I used:
- *t<400* for datasubset1 (i.e. Case 1 where K >> N<sub>0</sub> and N<sub>t</sub> is small; this is a point in time prior to the population plateauing)
- *t>1000* for datasubset2 (i.e. Case 2 where N<sub>t</sub> = K; this is a point in time after the population reaches carrying capacity, K)

This plot shows the logistic growth data with vertical lines indicating t for Case 1 and Case 2 📈

![Plot showing Logistic Growth Data with Vertical Lines Indicating t for Case 1 and Case 2 📈](https://github.com/sathvikakrishnan/logistic_growth/blob/main/plot.png?raw=true)

From this, I extracted:
- N<sub>0</sub> = 7.5907133 This is the intercept of summary of model 1 from datasubset1 (linear model)
  
- r = 0.0299202 This is the gradient of summary of model 1 from datasubset1 
  
- K = 1000000000 This is the intercept of summary of model 2 from datasubset2

*Question 2*

Assuming exponential population growth:
When t=4980 min, N<sub>t</sub>=3.902005 &times; 10<sup>65</sup>

Assuming logistic population growth:
When t=4980 min, N<sub>t</sub>=1 &times; 10<sup>9</sup>

We can see that if we use the exponential model for population growth, we get a population size that extensively exceeds the carrying capacity (K). In fact, the answer is 3.902005 &times; 10<sup>56</sup> times larger than the carrying capacity (which is 1000000000). This is contrasted by the logistic growth model. In this model, there is a carrying capacity so the population plateaus out at 1000000000. Therefore, even at a large time point of t=4980, the population remains at carrying capacity. This difference between models can be explained biologically: the exponential models assume unlimited resources, constant birth and death rates, no density-dependent factors, and constant environmental conditions. As a result of all these assumptions, particularly the lack of density-dependent factors, the population is allowed to grow ad infinitum. This is biologically unreasonable. The logistic model does not make these assumptions as it has a carrying capacity (i.e. the equilibrium population size where the available resources in an ecosystem are sufficient to sustain the population given limited resources and density-dependent regulation).

*Question 3*





x<sup>2</sup>
H<sub>2</sub>O