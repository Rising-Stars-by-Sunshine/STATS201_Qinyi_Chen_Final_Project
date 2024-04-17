# Applying Decoded Neurofeedback and Hyperalignment in moter-related brain patterns

## Project Information
- **Author**: Qinyi Chen, Behavioral Science/Neuroscience, Class of 2026, Duke Kunshan University
- **Instructor**: Professor Luyao Zhang, Duke Kunshan University
- **Disclaimer**: This project is a submission to the Final Project for STATS201 Introduction to Machine Learning for Social Science, 2023 Autumn Term (Seven Week - Second) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I extend my sincere gratitude to Professor Luyao (Sunshine) Zhang for her invaluable supervision and insightful teaching during the STATS 201 machine learning for social science course. Her guidance and support were instrumental in shaping the development of this project. Additionally, I would like to express my thanks to my peers in STATS 201 for fostering a collaborative environment that greatly enriched my educational journey.

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
6. [Spotlight](#spotlight)
7. [More about the Author](#more-about-the-author)
8. [References](#references)

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
Provide details on data sources and usage.

### Code
[code](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/code)

### Results
**Model Accuracy**: 0.5625

**Correlation**:
![Correlation](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/code/Correlation.png)


### Spotlight
Highlight unique contributions, media appearances, etc.

### More about the Author
- **Headshot**: [Insert headshot]
- **Self-introduction**
- **Final Reflections**
  - Intellectual growth
  - Professional growth
  - Living a purposeful life

### References
- **Data Source**: [BNCI 2014-001 Motor Imagery dataset. Dataset](https://paperswithcode.com/dataset/bci-competition-4-version-iia)
- **Code Source**: [Provide URL to your code repository]
- **Article Sources**:
  - Shibata, Kazuhisa, et al. "Toward a Comprehensive Understanding of the Neural Mechanisms of Decoded Neurofeedback." NeuroImage 188 (2019): 539–56. https://doi.org/10.1016/j.neuroimage.2018.12.022.
  - Taschereau-Dumouchel
