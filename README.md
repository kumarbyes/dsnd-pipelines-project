# Identification of trending products by analysing Customer reviews

![Classification](images/Classification.png)

## Table of Contents

- [Project Description](#project-description)
- [Dataset](#dataset)
- [Requirements](#Requirements)
- [Installations](#Installations)
- [File description](#file-description)
- [Result summary](#Result-summary)
- [License](#license)

## Project Description

This project is used to predict whether a customer recommends the product using Sklearn python library. As the given dataset contains numerical, categorical and text columns, preprocessing is performed separately on the columns. Text columns were explored and preprocessed using SpaCy. After preprocessing, the text columns were converted to numerical columns using TFIDF Vectorizer and DictVectorizer. Once all the columns were numerical, model fitting and prediction was performed using Support Vector classification. Considering the compute power required for finetuning, model hyperparameters were tuned using RandomSearchCV. Finally the models were compared using the evaluation metrics available in Sklearn.

### Dataset

The dataset has been anonymized and cleaned of missing values.

There are 8 features for to use to predict whether a customer recommends or does
not recommend a product.
The `Recommended IND` column gives whether a customer recommends the product
where `1` is recommended and a `0` is not recommended.
This is your model's target/

The features can be summarized as the following:

- **Clothing ID**: Integer Categorical variable that refers to the specific piece being reviewed.
- **Age**: Positive Integer variable of the reviewers age.
- **Title**: String variable for the title of the review.
- **Review Text**: String variable for the review body.
- **Positive Feedback Count**: Positive Integer documenting the number of other customers who found this review positive.
- **Division Name**: Categorical name of the product high level division.
- **Department Name**: Categorical name of the product department name.
- **Class Name**: Categorical name of the product class name.

The target:

- **Recommended IND**: Binary variable stating where the customer recommends the product where 1 is recommended, 0 is not recommended.

### Requirements

-**Python Version**: 3.11.9 was used for this project<br/>
-Jupyter notebook was used for the complete development of this project<br/>
-Check Requirements.txt file for all the libraries used in the project<br/>

### Installation

Install the required libraries for the project using **requirements.txt** file:

```bash
pip install -r requirements.txt
```

### File description

Following files are available in the github repository to succesfully run the code:

1. **starter.ipynb**: This is primary file containing all the relevant python code for project. At each point in the notebook, markdown cells are added to explain the process or inform about the inference.
2. **Requirements.txt**: Python libraries used in the project for pip install
3. **reviews.csv**: Csv file containing the data needed for the machine learning models
4. **LICENSE.txt**: License file for the project

### Result Summary

## License

[License](LICENSE.txt)
