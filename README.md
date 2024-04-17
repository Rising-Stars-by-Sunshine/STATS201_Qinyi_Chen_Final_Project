# Applying Decision Tree to Investigate How Personality Traits Influence Rational Decision-Making Behaviors

## Project Information
- **Author**: Qinyi Chen, Behavioral Science/Neuroscience, Class of 2026, Duke Kunshan University
- **Instructor**: Professor Luyao Zhang, Duke Kunshan University
- **Disclaimer**: This project is a submission to the Final Project for STATS201 Introduction to Machine Learning for Social Science, 2023 Autumn Term (Seven Week - Second) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: I extend my sincere gratitude to Professor Luyao Zhang for her invaluable supervision and insightful teaching during the STATS 201 machine learning for social science course. Her guidance and support were instrumental in shaping the development of this project. Additionally, I would like to acknowledge the helpful suggestions made by my peers in this class such as Yifei Luo in broadening my ideas, as well as my friends not in this course. Sincere gratitude to my roommate Yihan Wang and my friend Juntang Wang for helping me query datasets that are suitable for research. Moreover, thanks to my friend Chinyu Chen for helping me with the bugged code.

## Project Summary
**Applying Decision Tree to Investigate How Personality Traits Influence Rational Decision-Making Behaviors**
![chart](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Flow_chart.png)
*Flow Chart Created by Marksmap*

### Background/Motivation
In behavioral science, rationality describes a person's ability to make proper decisions by utilizing optimal outcomes, often by mitigating various cognitive biases. The study "Cognitive Biases and Mindfulness" (Maymin & Langer, 2021) delved into the relationship between mindfulness and rationality. It surveyed participants on 22 cognitive biases across three conditions: Mindful, Mindequal, and Mindless, alongside conducting the Langer Mindfulness Survey (LMS) to measure personality traits influencing rational decision-making. The study concluded that a mindful state could enhance performance by reducing cognitive biases and making rational decisions. 

### Research Questions
How do different personality traits correlate with rational decision making behaviors?

### Application Scenarios
This research will be applicable in personal development, educational settings, and professional environments where decision-making and cognitive bias mitigation are critical.

### Methodology
**Model Building**
The study utilizes **Decision Tree models** to analyze the data. The X variable includes multiple personality traits, and the Y variable includes different aspects of rationality indexes. Under this circumstance, the Decision Tree is most suitable for modeling two variables containing multi-dimensional input.
**Data Visualization**
The correlation between total score of rationality and each personality trait was calculated. Feature importance plots are employed to visually explore the relationships between personality traits and rational decision-making capacities.

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
The data was found from [Wolfram Data Repository-Maymin--Langer-2021-Cognitive-Biases-and-Mindfulness](https://datarepository.wolframcloud.com/resources/Philip%20Z.%20Maymin_Data-for-Maymin--Langer-2021-Cognitive-Biases-and-Mindfulness/)

**Data dictionary**

**Table 1：Rationality Index**

| Variable Name            | Description                                     | Research Question | Options | Rational Choice (2 points)|
|--------------------------|-------------------------------------------------|----------------|---------------|---------------|
| differentiating          | The ability to find the difference between two pictures|Can you spot the missing fruit? ![missing_fruit](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Data/differenciating.png)| A: Yes, I see the missing fruit; B: No, I don’t see the missing fruit; C: No, I don’t think there is a missing fruit | A: Yes, I see the missing fruit|
| illusion_debiasing       | Ability to discriminate biased illusion (e.g. vase or faces) | What can you see here? ![Vase](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Data/Vase.png)|A: I see a vase. B: I see two faces. C: I see both a vase and the two faces. |C: I see both a vase and the two faces.|
| loss_aversion            | Tendency of feeling the pain from losses twice as much as they feel the pleasure from gains.|Suppose you had to choose one of these two options. Which would you prefer?| a. You get $20 for sure. b. You toss a fair coin. Heads you get $300. Tails you lose $100.|b. You toss a fair coin. Heads you get $300. Tails you lose $100.|
| hyperbolic_discounting   | The ability to reject current profit to delayed gratification | Would you prefer to receive $1500 today or $1800 1 month from now? |a. $1500 today; b. $1800 1 month from now| b. $1800 1 month from now|
| conjunction_fallacy      | erroneously view a specific event as more likely than a more general event  | Linda is 31 years old, single, outspoken, and very bright. She majored in philosophy. As a student, she was deeply concerned with issues of discrimination and social justice, and also participated in anti-nuclear demonstrations. Which is more probable?|  a. Linda is a bank teller; b. Linda is a bank teller and is active in the feminist movement|a. Linda is a bank teller|
| gambling_fallacy       | Tendency to expect a surprising but short run of heads to change the outcome of future coin tosses | If you toss a coin five times and it comes up heads all five times, what do you think will happen if you toss it one more time? | a. More likely to come up tails b. Equally likely to come up heads or tails c. More likely to come up heads | b. Equally likely to come up heads or tails |
| confirmation_bias      | Tendency to seek evidence that confirms one's beliefs rather than disprove them | You are given four cards, each with a letter on one side and a number on the other. Which cards would you turn over to check if the rule "Any card with a vowel on one side has an even number on the other side" is true? ![cards](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Data/confirmation.png)| a. Turn over card 3 only. b. Turn over cards 1, 2, 3, and 4. c. Turn over cards 3 and 4 only. d. Turn over cards 1, 3, and 4 only. e. Turn over cards 1 and 3 only. |c. Turn over cards 3 and 4 only. |
| positional_bias        | Over-weighting relative vs. absolute value in decision making, particularly in comparing incomes | Which job offer would you prefer, assuming no other differences between the opportunities? a. A job paying $44,000 in a firm where the average salary is $50,000 b. A job paying $42,000 in a firm where the average salary is $38,000 | a. A job paying $44,000 in a firm where the average salary is $50,000 b. A job paying $42,000 in a firm where the average salary is $38,000 | a. A job paying $44,000 in a firm where the average salary is $50,000 |
| emotional_attachment  | Attachment to possessions based on emotional value      | You bought a ticket to a sold-out concert for $200. Richer or more desperate fans on the internet would pay up to $3000 for your ticket. Would you sell it? | a. Yes, I would sell it b. No, I would not sell it                                           | b. Yes, I would sell it  |
| fairness               | Evaluation of fairness in pricing strategy               | How would you rate the hardware store's action of raising the price of snow shovels after a large snowstorm? | a. Completely fair b. Acceptable c. Unfair d. Very unfair | c. Unfair |
| availability_bias      | Biased perception of likelihood based on ease of recall  | Is the letter R more likely to appear as the first letter or as the third letter in a word?             | a. R is more likely to appear as the first letter in a word b. R is more likely to appear as the third letter in a word | a. R is more likely to appear as the first letter in a word |
| equiprobability_illusion | Misjudgment of probabilities based on past outcomes    | Who do you now think is the pro among Al, Bob, and Carl after the given scenario?                        | a. Al b. Bob c. Carl                                                                     | a. Al |
| representativeness_bias| Biased evaluation based on stereotypical traits         | Is Steve more likely to be a librarian or a farmer based on the description provided?                     | a. Librarian b. Farmer                                                                   | a. Librarian |
| endowment_effect       | Tendency to overvalue items due to ownership            | Would you sell your lottery ticket for $2 after someone offers to buy it from you?                        | a. Yes b. No                                                                              | b. No |
| leaping_to_conclusions | Tendency to rush to conclusions without considering all options | Which of the shapes provided does not belong? ![leap](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Data/leap.png)                                                       | a. A b. B c. C d. D e. E                                                                | c. C |
| disposition_effect     | Tendency to hold onto losing positions too long         | What do you want to do with the shares of stock that you currently own after its price has dropped?       | a. Hold on until the price gets back to $50 or higher, then sell b. Sell now c. Sell if it drops even lower to $15, or if it gets back up to $50 | b. Sell now |


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

On average, the model correctly predicts approximately 56.25% of the labels across all the samples in the test set. This accuracy is lower than expected but still acceptable. 

The lower prediction accuracy can be possibly due to the complexity of both X and Y variables. In the personality traits, there are often 2 or 3 questions inquiring about the same personality traits, yet the answer made by participants still changes slightly. The explanation of this phenomenon is some mis-interpreted self-evaluation, and that interferes with the modeling process.

Additionally, the low accuracy can also be attributed to the raw data processing period. Since it is not appropriate to clean all the NaNs in this dataset, which will return a relatively tiny database, I dropped some columns that contain too many NaNs in both rationality and personality. Additionally, I artificially filled some still-existing NaNs with 0 (the scale leans to less rationality). This may lead to an underestimation of the overall rationality. Therefore, if the research can be conducted again with completed database, the accuracy of the model should increase. 

**Correlation:**

![Correlation](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Code/Correlation.png)

- **Rationality and Personality**

**Strong Negative Correlation**: *total_rationality_score* has a strong negative correlation with *Less_creative* (r = -0.10), and *Low_novelty_seeking* (r = -0.19), suggesting that higher rationality is associated with being more creative and seeking novelty.
**Strong Positive Correlation:** *total_rationality_score* has a relatively strong positive correlation with *Curiosity* and willingness to take on new intellectual challenges *Intellectual_challenge*, which indicates that curious and intellectually active people tend to perform more rationally.
- **Within Personality Traits**
  
**Strong Positive Correlations**: There are several variables that show strong positive correlations with each other, for instance:
Creativity and Curiosity (r = 0.53)
Creativity and Novelty_methods (r = 0.51)
Intellectual_challenge and Aspiration_to_knowledge (r = 0.64)
These strong positive correlations indicate that as one trait increases, the other does too, for example, those who enjoy intellectual challenges also aspire to gain knowledge.


### References
- **Data Source**: [Wolfram Data Repository-Maymin--Langer-2021-Cognitive-Biases-and-Mindfulness](https://datarepository.wolframcloud.com/resources/Philip%20Z.%20Maymin_Data-for-Maymin--Langer-2021-Cognitive-Biases-and-Mindfulness/)
- **Code Source**: [Final_Project_notebook](https://github.com/Rising-Stars-by-Sunshine/STATS201_Qinyi_Chen_Final_Project/blob/main/Code/Final_Project_Qinyi_Cognitive_Bias_and_Personality.ipynb)
- **Article Sources**:Maymin, Philip Z., and Ellen J. Langer. “Cognitive Biases and Mindfulness.” Humanities and Social Sciences Communications 8, no. 1 (February 3, 2021). [https://doi.org/10.1057/s41599-021-00712-1](https://doi.org/10.1057/s41599-021-00712-1). 
