# Fraud-Detection-for-Accenture-Classification

[![View Repositories](https://img.shields.io/badge/View-My_Repositories-blue?logo=GitHub)](https://github.com/ikoghoemmanuell?tab=repositories)
[![View My Profile](https://img.shields.io/badge/MEDIUM-Article-purple?logo=Medium)](https://medium.com/@emmanuel.ikogho/classification-predicting-sepsis-with-machine-learning-and-fastapi-3a3d05d0b5b4)
[![Docker App](https://img.shields.io/badge/Docker-App-yellow)](https://huggingface.co/spaces/ikoghoemmanuell/Sepsis-Prediction-With-FastAPI)
[![Website](https://img.shields.io/badge/My-Website-darkgreen)](https://emmanuelikogho.netlify.app/)

Develop a Machine Learning API (Application Programming Interface) using FastAPI.

![alt text](image.png)

## Introduction

We will develop a model for predicting fraudulent transactions for a
financial company and use insights from the model to develop an actionable plan. Data for the
case is available in CSV format having 6362620 rows and 10 columns.
Candidates can use whatever method they wish to develop their machine learning model.
Following usual model development procedures, the model would be estimated on the
calibration data and tested on the validation data. This case requires both statistical analysis and
creativity/judgment.

## Description

## Importance of Project  

The dataset used contains a list of patients in a hospital and their attributes and whether the patient is positive for Sepssis or not.

Sepsis is a severe and potentially life-threatening condition that occurs when the body's response to an infection triggers widespread inflammation. It is often referred to as blood poisoning.

The aim of this project is to explore the various factors that can cause sepsis in order to predict the occurence of sepsis.

Predicting sepsis is important because early recognition and intervention can significantly improve patient outcomes. Sepsis can progress rapidly and become life-threatening within a short period. By identifying patients who are at risk of developing sepsis, healthcare providers can initiate timely treatment and interventions to prevent the condition from worsening.

# Dataset Description -

The data for this project is in a csv format. The following describes the columns present in the data.

| Column Name    | Target | Description                                                                                                                                                                                                              |
| -------------- | ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| step           | N/A    | Maps a unit of time in the real world. In this case, 1 step is 1 hour of time. Total steps 744 (30 days simulation).                                                                                                     |
| type           | False  | Type of transaction: CASH-IN, CASH-OUT, DEBIT, PAYMENT, and TRANSFER.                                                                                                                                                    |
| amount         | False  | Amount of the transaction in local currency.                                                                                                                                                                             |
| nameOrig       | False  | Customer who started the transaction.                                                                                                                                                                                    |
| oldbalanceOrg  | False  | Initial balance before the transaction.                                                                                                                                                                                  |
| newbalanceOrig | False  | New balance after the transaction.                                                                                                                                                                                       |
| nameDest       | False  | Customer who is the recipient of the transaction.                                                                                                                                                                        |
| oldbalanceDest | False  | Initial balance of the recipient before the transaction. Note that there is no information for customers that start with M (Merchants).                                                                                  |
| newbalanceDest | False  | New balance of the recipient after the transaction. Note that there is no information for customers that start with M (Merchants).                                                                                       |
| isFraud        | True   | Indicates if the transaction is fraudulent. Fraudulent transactions aim to profit by taking control of customers' accounts and emptying the funds by transferring to another account and then cashing out of the system. |
| isFlaggedFraud | False  | Indicates if the transaction was flagged as suspicious for transferring more than 200,000 in a single transaction.                                                                                                       |

## Setup

Install the required packages to be able to run the evaluation locally.

You need to have [`Python 3`](https://www.python.org/) on your system (**a Python version lower than 3.10**). Then you can clone this repo and being at the repo's `root :: repository_name> ...` follow the steps below:

- Windows:

```python
python -m venv venv; venv\Scripts\activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt
```

- Linux & MacOs:

```python
python3 -m venv venv; source venv/bin/activate; python -m pip install -q --upgrade pip; python -m pip install -qr requirements.txt
```

The both long command-lines have a same structure, they pipe multiple commands using the symbol `;` but you may manually execute them one after another.

1. **Create the Python's virtual environment** that isolates the required libraries of the project to avoid conflicts;
2. **Activate the Python's virtual environment** so that the Python kernel & libraries will be those of the isolated environment;
3. **Upgrade Pip, the installed libraries/packages manager** to have the up-to-date version that will work correctly;
4. **Install the required libraries/packages** listed in the `requirements.txt` file so that it will be allow to import them into the python's scripts and notebooks without any issue.

**NB:** For MacOs users, please install `Xcode` if you have an issue.

## Run FastAPI

To run the fastAPI, paste this code to your terminal:

```python
uvicorn main:app — reload
```

When you run the script and start the web server using Uvicorn, your FastAPI application becomes accessible at

```python
http://127.0.0.1:8000
```

To access the documentation of your API, you can simply add “/docs” to the URL:

```python
http://127.0.0.1:8000/docs
```

## Screenshots

![ezgif com-optimize (1)](https://github.com/ikoghoemmanuell/Machine-Learning-API-using-FastAPI/assets/102419217/a8352c5f-afea-43b1-8bf5-c24607cf3481)
![ezgif com-crop](https://github.com/ikoghoemmanuell/Machine-Learning-API-using-FastAPI/assets/102419217/df0ed5a8-2daf-47ca-a4f5-e6128429d5d3)

## Resources

Here are some ressources you would read to have a good understanding of FastAPI :

- [Tutorial - User Guide](https://fastapi.tiangolo.com/tutorial/)
- [Video - Building a Machine Learning API in 15 Minutes ](https://youtu.be/C82lT9cWQiA)
- [FastAPI for Machine Learning: Live coding an ML web application](https://www.youtube.com/watch?v=_BZGtifh_gw)
- [Video - Deploy ML models with FastAPI, Docker, and Heroku ](https://www.youtube.com/watch?v=h5wLuVDr0oc)
- [FastAPI Tutorial Series](https://www.youtube.com/watch?v=tKL6wEqbyNs&list=PLShTCj6cbon9gK9AbDSxZbas1F6b6C_Mx)
- [Http status codes](https://www.linkedin.com/feed/update/urn:li:activity:7017027658400063488?utm_source=share&utm_medium=member_desktop)

## 👏 Support

If you found this article helpful, please give it a clap or a star on GitHub!

## Author

- [Emmanuel Ikogho](https://www.linkedin.com/in/emmanuel-ikogho-6b959b24b/)
