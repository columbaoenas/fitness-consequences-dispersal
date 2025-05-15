# fitness-consequences-dispersal

Code files used for models and stats tests for my MBiol project, "Fitness consequences of dispersal: insights from a great tit population".

All code is provided as RMarkdown files, but I have not shared the data used to make calculations. The RProject file is provided as final_dispersal_project.RProj. Files are divided between initial data filtering and exploration, the three main questions, and the follow up analysis on dispersal distances.

### **Data filtering and exploration**

I produded two datasets from breeding and ringing records in Wytham Woods, to compare fitness at the scale of breeding attempts and lifetimes. The data pipeline used can be found in:
- final_data_pipeline_full.Rmd

Before answering my three main questions, I tested whether there was assortative mating in this population by dispersal status. These tests can be found in:
- assortative_mating_tests.Rmd

### **(1) Are there differences in fitness between dispersing and locally-born birds?**

I compared the effects on fitness of the dispersal status of males, females, and breeding pairs. These models are divided between:
- final_fitness_females.Rmd
- final_fitness_males.Rmd
- final_fitness_par.Rmd

### **(2) Can differences between dispersing and locally-born birds be explained by the environment?**

I first compared if birds were found breeding in different environments based on their dispersal status. These models were divided between females and males, in:
- final_spatial_environmental_test_fem.Rmd
- final_spatial_environmental_test_male.Rmd

I then added these environmental variables to the fitness models in part (1) to determine if the effect size changed. They can be found in:
- final_spatial_fitness_fem.Rmd
- final_spatial_fitness_male.Rmd
- final_spatial_fitness_par.Rmd

### **(3) Do differences between dispersing and locally-born birds persist over lifetimes?**

To determine whether observed differences fade or persist as birds gain more breeding experience, I added a binary variable representing first/subsequent breeding attempts by an individual to models comparing the effect of dispersal status on fitness. These models were split between females and males, and can be found in:
- final_temporal_fitness_fem.Rmd
- final_temporal_fitness_male.Rmd

### **(4) Follow-up analysis: dispersal distance**

Finally, I aimed to determine if differences in recruitment could be explained by differences in natal dispersal distance in recruits based on the dispersal status of their parents. I fit three models to separate the effects of mothers, fathers, and pairs' effect on their offspring, all found in:
- recruit_distance_comparisons.Rmd
