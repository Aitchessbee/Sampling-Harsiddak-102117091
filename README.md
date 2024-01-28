# Sample Analysis
## Introduction to Sampling
Sampling is a valuable method employed for extracting insights about a population by analyzing statistics from a representative subset, thus avoiding the need to examine every individual. Addressing an initial dataset imbalance of 763 non-fraudulent cases and only 9 fraudulent cases, an oversampling approach was executed. This involved creating additional instances of the minority class (fraudulent cases) to align with the majority class (non-fraudulent cases), resulting in a balanced dataset consolidated into a single data frame.

Various sampling techniques were employed in this study:

- **Simple Random Sampling:** Involves the random selection of samples from the population.
- **Systematic Sampling:** Entails regular interval selection after a random start.
- **Cluster Sampling:** Encompasses randomly selecting clusters from the population.
- **Stratified Sampling:** Involves the division of the population into subgroups based on specific criteria.
- **Bootstrap Sampling:** Utilizes resampling with replacement to create multiple samples from the original dataset.

Following the generation of five distinct samples using these techniques, five models were applied to each sample. The accuracies of each model for a given sample are summarized in the table below:

| Sampling Technique      | Random Forest | Logistic Regression | Naive Bayes      | Decision Trees   | KNN              |
|-------------------------|---------------|---------------------|------------------|------------------|------------------|
| Simple Random Sampling  | 0.9870        | 0.8831              | 0.7013           | 0.9610           | 0.8701           |
| Systematic Sampling     | 1.0000        | 0.8926              | 0.7450           | 1.0000           | 0.9329           |
| Cluster Sampling        | 1.0000        | 0.9670              | 1.0000           | 1.0000           | 0.9890           |
| Stratified Sampling     | 1.0000        | 0.9030              | 0.7239           | 0.9925           | 0.9552           |
| Bootstrap Sampling      | 1.0000        | 0.9250              | 0.7500           | 0.9625           | 0.9375           |

In the table above, each row corresponds to a sampling technique, and each column represents the accuracy achieved by each model applied to the respective sample generated using that particular technique.
<br>
### Notably, the RANDOM FOREST model demonstrated superior performance, particularly when applied to the Stratified Sampling Technique.
