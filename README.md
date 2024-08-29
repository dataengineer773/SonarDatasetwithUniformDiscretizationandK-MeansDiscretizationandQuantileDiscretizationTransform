We want to use Uniform Discretization Transform and K-Means Discretization TRansform and Quantile Discretization TRansform an in the final we choose thenumber as an arbitrarry number and in this case  10 
This hyperparameter can be tuned to explore the effect of the resolution of the the transform on the  resulting skill of the model, a uniform discretization transform will preserve the probability distribution
of each input variable but will make it discrte with the specefic number of online of labels, we can apply the uniform discretization transform using  the KBinsDiscretizer class and setting the strategy 
argument to uniform and in the next step we use a K-means discretization will attepmt to fit k clusters for each input variable amd assign each observation to a cluster and on the next step we use a quantile 
discretization transform will attempt to split the observation for each input variable into k groups, where the number of observations siigned to each is approximately equal unless there are a large number of
observations or a complex empirical distribution ant in the final we explore our models.
