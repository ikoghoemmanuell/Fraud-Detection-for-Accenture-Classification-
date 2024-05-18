# Fraud-Detection-for-Accenture-Classification

[![View Repositories](https://img.shields.io/badge/View-My_Repositories-blue?logo=GitHub)](https://github.com/ikoghoemmanuell?tab=repositories)
[![View My Profile](https://img.shields.io/badge/MEDIUM-Article-purple?logo=Medium)](https://medium.com/@emmanuel.ikogho/classification-predicting-sepsis-with-machine-learning-and-fastapi-3a3d05d0b5b4)
[![Website](https://img.shields.io/badge/My-Website-darkgreen)](https://emmanuelikogho.netlify.app/)

![alt text](image.png)

## Introduction (What is Fraud?)

Fraud is much more common than you think and can happen to any business. Spotting and stopping fraud early can prevent losses, reputational damage, and might even save your business from collapse.

Put simply, fraud is stealing by deception. If someone lies to you in order to steal money, property, or data, they may have committed fraud.

In this project, we will develop a model for predicting fraudulent transactions for a financial company and then use insights from the model to develop a plan of action.

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

## 👏 Support

If you found this article helpful, please give it a clap or a star on GitHub!

## Author

- [Emmanuel Ikogho](https://www.linkedin.com/in/emmanuel-ikogho-6b959b24b/)
