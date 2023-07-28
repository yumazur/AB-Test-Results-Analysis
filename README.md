# AB-Test-Results-Analysis
Checking the data for compliance with the terms of reference for the AV test. Identification of errors in the division of participants into test and control groups. Build a sales funnel. Visualized the effect of the experiment. Hypotheses about the equality of the proportions of funnel stages were tested.
### Objective: 
Check the correctness of the A / B test for the implementation of an improved recommender system in accordance with the terms of reference, analyze the results. Expected effect: within 14 days from the moment of registration in the system, users will show an improvement in each metric by at least 10%.
### Skills and tools:
Python, Pandas, Seaborn, Plotly, SciPy, A/B testing, testing of statistical hypotheses
### Examples of visualizing data from a project:
![ABtestProject](https://github.com/yumazur/AB-Test-Results-Analysis/assets/140715941/985e7417-e801-4f39-ada4-dd565dcf2512)

### Analysis results:
* An increase in metrics by 10% in the experimental group was not recorded. The introduction of a new recommender system did not lead to the desired results. The test did not show a significant increase in any of the metrics (conversions to view product cards - product_page event, cart views - product_cart, purchases - purchase). And at the product_page and purchase steps, the values of the experimental group turned out to be noticeably worse than in the control group. We can assume that the experiment had a negative impact on user behavior. Only at the product_cart stage did group B grow relative to group A.
* Results in group B relative to group A:
     * conversion to view product cards - product_page event - 86%
     * cart views - product_cart - 107.3%
     * purchases - purchase - 95.6%
     * in groups A and B, the conversion at the purchase stage exceeds 100% (107%, 102%). These values require additional analysis to understand the reasons for such results.

In addition, exploratory analysis revealed anomalies in the process of recruiting users into groups. The average purchase price in group B is lower than in group A. Sales in the experimental group are worse than in the control group.

**Conclusion:**

The experiment did not meet the requirements of the terms of reference for the A / B test, did not show the desired results and led to negative changes at some steps of the funnel. More careful planning and control of the experiment is recommended to obtain more reliable results. At the end of the study, recommendations are given for the correct preparation and conduct of the test.
