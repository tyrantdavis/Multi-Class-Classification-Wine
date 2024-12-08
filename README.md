# Building a Multinomial Logistic Regression - Wine

Multi-Class Classification Model

---

## Introduction
Professors at a college are eager to integrate machine learning into their respective disciplines. The Chemistry department aims to enhance students' understanding of the interactions among various chemical compounds. Specifically, students will investigate how minor alterations in a substance's chemical composition can influence its overall characteristics.

A faculty member from the Chemistry department has shared a dataset containing information on different wines, each characterized by multiple attributes. Each wine entry is categorized according to its specific cultivar. However, in contrast to the previous classification project, this dataset allows for categorization into three distinct classes rather than just two. Therefore, a binary classification model will not suffice; a multi-class classification model must be developed to accurately predict the type of wine represented by each sample.

This examination will allow classifying wines as being a particular type.

This project will scope, analyze, prepare, plot data, and seek to explain the findings from the analysis.

**Feature Information**

- Alcohol
- Malic acid
- Ash
- Alcalinity of ash
- Magnesium
- Total phenols
- Flavanoids
- Nonflavanoid phenols
- Proanthocyanins
- Color intensity
- Hue
- OD280/OD315 of diluted wines
- Proline
- target - wine type / region of origin: 0, 1, or 2
  
Here are a couple of questions that this project seeks to answer:

- What are key factors influencing wine classification?
- Which category has the highest count?
- Which category has the lowest count?

### Scenario
You are employed in the Chemistry department at a state college, where an upcoming lecture will delve into the chemistry of wine and its analysis. The  department is dedicated to improving students' comprehension of the relationships between different chemical compounds. In particular, students will explore how slight changes in a substance's chemical makeup can affect its overall properties. Rather than simply delivering a traditional lecture and expecting students to absorb the information passively, you intend to encourage them to draw their own conclusions and validate those insights through practical engagement. To achieve this, you plan to develop a machine learning model that will facilitate this exploration. Utilizing a real-world dataset containing diverse statistics about wine, the model will classify each individual wine as a specific type. 

**Data Sources:**

- [UCI ML Wine](https://archive.ics.uci.edu/dataset/109/wine)
  

## Project Goals
The goal is to determine the specific variety of wine that each sample represents.

#### Why use a multinomial logistic regression algorithm to predict the outcome?
Multi-class classification involves categorizing a data instance into one specific class from a set of three or more options, which aligns well with the objectives of this project. One effective approach to address multi-class challenges is through the use of Multinomial Logistic Regression. This form of regression determines the class with the highest probability, where all probabilities add up to 1. Multinomial Logistic regression is therefore appropriate for addressing classification issues in situations where traditional binary regression is inadequate.


## Data
An anonymized dataset that can be used to train the machine-learning model has been found. It is a CSV file containing 178 wine records. 


## Conclusions
- What are key factors influencing wine classification?
    -  flavanoids has an inverse relation to target. It is the overall number one attribute influencing class with a -85% correlation to target
    -  alcalinity_of_ash is the number one positive attribute influencing class at 52%
    
- Which category has the highest count?
    - Category 1 has the highest class count at 71. 
- Which category has the lowest count?
    - Category 2 has the lowest class count at 48. 