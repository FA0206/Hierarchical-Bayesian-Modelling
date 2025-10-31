# Thoughts Dump
0. Major data cleaning to be done. Lot of NA values need to be handled. Also need to convert ordinal and nominal variables to numbers and store that dictionary somewhere (a json or maybe smth else, need to consider ideas for this).

1. It seems SalePrice in the Ames dataset is VERY right skewed. Need to plot that and model log(SalePrice) instead of SalePrice itself.

2. Crawl, Walk, Run Approach
	a. Crawl: Baseline Models - Basic Ridge / Lasso regression for a monolithic pool as well as a per neighborhood model. (This is non-Bayesian and the per neighborhood models should be unstable)
	b. Walk: Simple Bayesian Models - Bayesian Linear Regression for pooled and non-pooled data. 
	c. Hierarchical Model: Partial Pooling - Need to figure out the math and working behind this.

3. What visualizations do I want?
	a. A bar chart showing the number of sales per neighborhood (to justify the need for the project)
	b. A "forest plot" or a "caterpillar plot" comparing the various models (baseline, to simple bayesian to hierarchical bayesian)
	c. Posterior predictive plots to show that the model captures the data's distribution
