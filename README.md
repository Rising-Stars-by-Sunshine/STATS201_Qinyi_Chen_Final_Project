# Applying Decoded Neurofeedback and Hyperalignment in moter-related brain patterns

## Project Information
- **Author**: Qinyi Chen, Behavioral Science/Neuroscience, Class of 2026, Duke Kunshan University
- **Instructor**: Professor Luyao Zhang, Duke Kunshan University
- **Disclaimer**: This project is a submission to the Final Project for STATS201 Introduction to Machine Learning for Social Science, 2023 Autumn Term (Seven Week - Second) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I extend my sincere gratitude to Professor Luyao Zhang for her invaluable supervision and insightful teaching during the STATS 201 machine learning for social science course. Her guidance and support were instrumental in shaping the development of this project. Additionally, I would like to acknowledge the helpful suggestiong made by my peers in this class such as Yifei Luo in broadening my ideas, as well as my friends not in this course. Sincere gratitude to my roommate Yihan Wang and my friend Juntang Wang in helping me querying database that is suitable for research. Moreover, thanks to my friend Chinyu Chen in helping me with the bugged code.

## Project Summary
**Applying Decision Tree to Investigate How Personality Traits Influence Rational Decision Making Behaviors**

### Background/Motivation
In behavioral science, rationality describes a person's ability to make proper decisions by utilizing optimal outcomes, often by mitigating various cognitive biases. The study "Cognitive Biases and Mindfulness" (Maymin & Langer, 2021) delved into the relationship between mindfulness and rationality. It surveyed participants on 22 cognitive biases across three conditions: Mindful, Mindequal, and Mindless, alongside conducting the Langer Mindfulness Survey (LMS) to measure personality traits influencing rational decision-making. The study concluded that a mindful state could enhance performance in reducing cognitive biases and making rational decisions. 

### Research Questions
How do different personality traits correlate with rational decision making behaviors?.

### Application Scenarios
This research will be applicable in personal development, educational settings, and professional environments where decision-making and cognitive bias mitigation are critical.

### Methodology
**Model Building**
The study utilizes **Decision Tree models** to analyze the data. The X variable includes multiple personality traits, and the Y variable includes different aspects of rationality indexes. Under this circumstances, Decision Tree is most suitable for modeling two variables containing multi-dimentional input.
**Data Visualization**
The correlation between total score of rationality and each personality traits were calculated. Feature importance plots are employed to visually explore the relationships between personality traits and rational decision-making capacities.

## Intellectual Merits and Practical Impacts
- **Development of a Machine Learning Model of Rationality:** By integrating personality traits and rational decision-making metrics into a predictive model, this research contributes to the quantitative understanding of human behavior in decision sciences.
- **Exploration of Correlations:** This project seeks to uncover potential correlations between rationality and various personality traits, offering a deeper understanding of how inherent characteristics influence decision-making processes.
- **Practical Recommendations for Personal and Professional Growth:** The findings could provide actionable insights for individuals to adapt certain personality traits in work settings or other critical situations, fostering self-improvement and enhancing decision-making efficacy.

## Table of Contents
1. [Literature](#literature)
2. [Method](#method)
3. [Data](#data)
4. [Code](#code)
5. [Results](#results)
6. [References](#references)

### Literature
Maymin, Philip Z., and Ellen J. Langer. “Cognitive Biases and Mindfulness.” Humanities and Social Sciences Communications 8, no. 1 (February 3, 2021). [https://doi.org/10.1057/s41599-021-00712-1](https://doi.org/10.1057/s41599-021-00712-1). 

### Method
**Research Question Formulation**
- **Objective:** The primary objective of this research is to explore and identify potential correlations between various personality traits and cognitive biases using machine learning techniques.
- **Significance:** This question is crucial as it could provide insights into how intrinsic personality factors influence cognitive biases, potentially informing psychological and behavioral interventions.
**Operational Measures**
- **Variables**
- **Dependent (Y):** Rationality indexes (evaluated by the ability to avoid multiple biases).
- **Independent (X):** Personality traits measured by a standardized personality inventory.
- **Data Type:** The dataset is cross-sectional, gathered from a series of assessments across a diverse population at a single point in time.
**Hypothesis Development**
- **Prediction Hypothesis:** It's hypothesized that certain personality traits such as openness and neuroticism are predictive of the extent to which an individual exhibits specific cognitive biases.
- **Justification:** Previous research suggests that personality traits can influence decision-making processes and vulnerability to cognitive biases.
- **Machine Learning Algorithm Selection:** Decision Trees and Random Forests were selected due to their efficacy in handling non-linear relationships and interactions between multiple predictors, which is typical in psychological data.
**Model Development**
- **Data Processing:** The data were cleaned for missing values and outliers, and variables were normalized to ensure uniform scale. Feature engineering was conducted to create interaction terms that might reveal complex associations.
**Results Presentation**
- **Training and Testing:** The model was trained on 70% of the data with the remaining 30% used for testing. Performance metrics and confusion matrices were used to evaluate outcomes.
- **Data Visualization:** Results were visualized using ROC curves, precision-recall curves, and feature importance plots to illustrate the contributions of different variables.
**Model Evaluation**
- **Evaluation Criteria:** The models were evaluated based on accuracy, precision, recall, and the area under the ROC curve (AUC).
- **Iterative Improvement:** Techniques such as hyperparameter tuning and cross-validation were employed to refine the models and improve their predictive accuracy.


### Data

**Data dictionary**
**Table 1：Rationality Index**

**Table 2: Personality Traits**
| Variable Name           | Inquiry Question                             | Max | Min | Mean     | STD      |
|-------------------------|----------------------------------------------|-----|-----|----------|----------|
| Less_creative           | I generate few novel ideas.                 | 7   | 0   | 3.541284 | 1.941420 |
| Novelty_producing      | I make many novel contributions.             | 7   | 1   | 4.275229 | 1.626582 |
| Engagement             | I seldom notice what other people are up to.| 7   | 1   | 2.853211 | 1.626321 |
| Low_novelty_seeking    | I avoid thought-provoking conversations.     | 7   | 1   | 2.293578 | 1.523293 |
| Creativity             | I am very creative.                          | 7   | 1   | 4.495413 | 1.636527 |
| Curiosity              | I am very curious.                           | 7   | 1   | 5.431193 | 1.529748 |
| Novelty_methods        | I try to think of new ways of doing things. | 7   | 1   | 5.348624 | 1.511537 |
| Agility                | I am rarely aware of changes.                | 7   | 1   | 2.311927 | 1.274372 |
| Intellectual_challenge | I like to be challenged intellectually.      | 7   | 1   | 5.550459 | 1.443287 |
| Creative_producing     | I find it easy to create new and effective ideas. | 7   | 1   | 4.587156 | 1.717077 |
| Insight_of_environment | I am rarely alert to new developments.       | 7   | 1   | 2.541284 | 1.384652 |
| Aspiration_to_knowledge| I like to figure out how things work.        | 7   | 1   | 5.394495 | 1.509343 |
| Conservative_thinking  | I am not an original thinker.                | 7   | 1   | 2.889908 | 1.657416 |


### Code
[Final_Project_notebook](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Code/Final_Project_Qinyi_Cognitive_Bias_and_Personality.ipynb)

### Results
**Model Accuracy: 0.5625**
On average, the model correctly predicts approximately 56.25% of the labels across all the samples in the test set. This accuracy is lower than expectation but still acceptable. 
The lower prediction accuracy can be possibly due to the complexity of both X and Y variables. In the personality traits, there are often 2 or 3 questions inquiring the same personality traits, yet the answer made by participants still changes slightly. The explanation of this phenomenon is some mis-interpreted self-evaluation, and that interferes with the modeling process.
Additionally, the low accuracy can also be attributed to the raw data processing period. Since it is not appropriate to clean all the NaNs in this dataset, which will return a relatively tiny database, I droped some columns that contains too much NaNs in both rationality and personality. Additionally, I artificially filled some still-existing NaNs with 0 (the scale leans to less rationality). This may lead to an underestimation of the overall rationality. Therefore, if the research can be conducted again with completed database, the accuracy of the model should increase. 
**Correlation:**
![Correlation](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Code/Correlation.png)


### References
- **Data Source**: [Wolfram Data Repository-Maymin--Langer-2021-Cognitive-Biases-and-Mindfulness](https://datarepository.wolframcloud.com/resources/Philip%20Z.%20Maymin_Data-for-Maymin--Langer-2021-Cognitive-Biases-and-Mindfulness/)
- **Code Source**: [Final_Project_notebook](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Code/Final_Project_Qinyi_Cognitive_Bias_and_Personality.ipynb)
- **Article Sources**:Maymin, Philip Z., and Ellen J. Langer. “Cognitive Biases and Mindfulness.” Humanities and Social Sciences Communications 8, no. 1 (February 3, 2021). [https://doi.org/10.1057/s41599-021-00712-1](https://doi.org/10.1057/s41599-021-00712-1). 
