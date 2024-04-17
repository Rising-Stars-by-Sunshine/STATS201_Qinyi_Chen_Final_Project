# Applying Decoded Neurofeedback and Hyperalignment in moter-related brain patterns

## Project Information
- **Author**: Qinyi Chen, Behavioral Science/Neuroscience, Class of 2026, Duke Kunshan University
- **Instructor**: Professor Luyao Zhang, Duke Kunshan University
- **Disclaimer**: This project is a submission to the Final Project for STATS201 Introduction to Machine Learning for Social Science, 2023 Autumn Term (Seven Week - Second) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I extend my sincere gratitude to Professor Luyao (Sunshine) Zhang for her invaluable supervision and insightful teaching during the STATS 201 machine learning for social science course. Her guidance and support were instrumental in shaping the development of this project. Additionally, I would like to express my thanks to my peers in STATS 201 for fostering a collaborative environment that greatly enriched my educational journey.

## Project Summary
Applying Decoded Neurofeedback and Hyperalignment in motor-related brain patterns.

### Background/Motivation
The intricate relationship between neural signals and consciousness has been a long-standing enigma in neuroscience. Recent advancements in computer science, particularly in big data and machine learning, have ushered in groundbreaking possibilities for deciphering how the brain responds to external stimuli. Notably, decoded neurofeedback (DecNef) has demonstrated its potential to induce targeted neural plasticity (Shibata et al., 2018) through data obtained from traditional fMRI methods. Additionally, hyperalignment, a technique designed to align and compare brain activities across individuals, holds promise in unraveling the correlations between sensory information and neuronal representations.

### Research Questions
This study focuses on applying hyperalignment in processing human motor imagery data to decode how brain signals represent motor patterns. Furthermore, decoded neurofeedback is applied to figure out potential pathways of clinical post-injury motor recovery.

### Application Scenarios
DecNef and hyperalignment are promising in enriching the theory of neuronal representation on external stimuli and behaviors. Moreover, the reinforcement technique can be used as a non-pharmacological intervention in several psychological disorders or neurological impairments.

### Methodology
The study will be analyzing the online EEG database of human motor imagery data (https://paperswithcode.com/dataset/bci-competition-4-version-iia). Based on the existing data, hyperalignment will be applied to align the brain patterns of 9 tested individuals. According to Taschereau-Dumouche (2018), a more detailed process of data processing includes applying pyMVPA 2.4 (www.pymvpa.org) in the NeuroDebian environment and using sparse logistic regression to select the best models.

### Results
This study will potentially identify the brain patterns representation of motor signals, shedding light on the neural basis of motor imagery. Besides, the result is an exploration of potential avenues for clinical treatment of brain-related motor injuries through Decoded Neurofeedback.

## Intellectual Merits and Practical Impacts
This research project holds significant intellectual and practical implications. Decoding brain signals related to motor imagery and recovery contributes to our understanding of neural representations. Furthermore, the potential applications of DeNef and hyperalignment techniques extend to non-pharmacological interventions in psychological disorders and neurological impairments, offering hope for improved clinical outcomes and patient well-being.

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
Provide references in Chicago Author-Date Style and BibTex here.

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
Provide links to repositories or embed code snippets.

### Results
Discuss results in detail.

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
