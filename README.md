# Analyze_ab_test_results_notebook
A/B tests are very commonly performed by data analysts and data scientists. 

## Introduction
A/B tests are very commonly performed by data analysts and data scientists. It is important that you get some practice working with the difficulties of these. For this project, you will be working to understand the results of an A/B test run by an e-commerce website. The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. Your goal is to work through this notebook to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

## Installation
You need to setup Jupyter Notebook on your computer. The following python packages (libraries) need to be installed. You can install these packages via conda or pip ... pip install <module_name>.

* Numpy
* Pandas
* Matplotlib
* Statsmodels
* Scipy
## Project Details
### Part I - Probability
Make some statistics to compute the probabilities of converting regardless of page, and analyze which page led to more conversions.

### Part II - A/B Test
Notice that because of the time stamp associated with each event, you could technically run a hypothesis test continuously as each observation was observed.

1. For now, consider you need to make the decision just based on all the data provided. If you want to assume that the old page is better unless the new page proves to be definitely better at a Type I error rate of 5%, what should your null and alternative hypotheses be? You can state your hypothesis in terms of words or in terms of p_old and p_new, which are the converted rates for the old and new pages.

2. Assume under the null hypothesis, p_new and p_old both have "true" success rates equal to the converted success rate regardless of page - that is p_new and p_old are equal. Furthermore, assume they are equal to the converted rate in ab_data.csv regardless of the page.

Use a sample size for each page equal to the ones in ab_data.csv.

Perform the sampling distribution for the difference in converted between the two pages over 10,000 iterations of calculating an estimate from the null.

### Part III - A regression approach
Perform Logistic regression to confirm results.

### Results
Based above calculation and during the A/B Test I see switch to the new page doesn't add any sense, because there is no statistical significance about increase conversion rate.
