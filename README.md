# CodePro-mlops-using-airflow-mlflow
>
> This project implements an end-to-end pipeline for CodePro Company to reduce the L2AC (Leads to Application Completion) to maximize profitability. We have implemented both Dev and Prod pipelines using Airflow and MLflow respectively. Experimentation has been doen using pycaret and mlflow. The project is deployed using airflow.

## Table of Contents

## General Information

### Problem Statement

CodePro is an EdTech startup that had a phenomenal seed A funding round.
It used the money to increase its brand awareness. As the marketing spending increased, it got several leads from different sources. Although it had spent significant money on acquiring customers, it had to be profitable in the long run to sustain the business.
The major cost that the company is incurring is the customer acquisition cost (CAC).
At the initial stage, customer acquisition cost is required to be high in companies. But as their businesses grow, these companies start focussing on profitability. Many companies first offer their services for free or provide offers at the initial stages but later start charging customers for these services. For example, Google Pay used to provide many offers, and Reliance Jio in India offered free mobile data services for over a year. Once these brands were established and brand awareness was generated, these businesses started growing organically. At this point, they began charging customers. Businesses want to reduce their customer acquisition costs in the long run.

We have chosen L2AC (Leads to Application Completion) as our business metric, as choosing L2P (Leads to Payment) will aggressively drop the leads.
A lead is generated when any person visits CodePro’s website and enters their contact details on the platform. A junk lead is generated when a person who shares their contact details has no interest in the product/service.
Having junk leads in the pipeline creates significant inefficiency in the sales process. Thus, the goal of the data Project is to build a system that categorises leads based on the likelihood of their purchasing CodePro’s course. This system will help remove the inefficiency caused by junk leads in the sales process.

### Pipeline Implemented

- Development Pipeline
  - Experimentation performed using pycaret tracked using mlflow to find baseline model
- Producion Pipeline
  - Data Pipeline
    - To fetch data from source and preprocess it for training and inference pipeline
  - Training Pipeline
    - In case of data drift under a threshold, retrain the model with new preprocessed data
  - Inference Pipeline
    - To predict the target variable for new data

## Technologies Used

- MLflow 1.29.0
- Airflow 1.7.0
- streamlit 1.8.0
- pycaret 2.3.1
- Pandas Profiling - 3.4.0
- Python version 3.8.8
- numpy library version 1.20.1
- pandas library version 1.2.4
- matplotlib library version 3.3.4
- seaborn library version 0.11.1
- git version 2.34.0.windows.1

## Contact

Created by [@sukhijapiyush] - feel free to contact me!

## License

This project is open source and available under the [Apache License].

## References

1. <https://pycaret.readthedocs.io/en/stable/>
2. <https://airflow.apache.org/docs/apache-airflow/stable/tutorial/fundamentals.html>
3. <https://www.mlflow.org/docs/latest/index.html>
4. <https://towardsdatascience.com/a-true-end-to-end-ml-example-lead-scoring-f5b52e9a3c80>
