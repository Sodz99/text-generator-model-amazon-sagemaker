# Build a Text Generator Model using Amazon SageMaker

- To understand text generation - To train and deploy the LSTM text generator model on amazon sagemaker

## Overview
Amazon sagemaker is a managed service on AWS cloud. It provides tools to deploy any Machine Learning algorithm on the cloud for predictive analysis. Data Scientist needs to deploy their built Machine Learning model in real-time, but they lack software engineering skills and rely on software engineers to deploy their model. On the other hand, Software engineers are not data scientists. Developing a full-scale ML service requires the developer to have a deeper understanding of the process, which is quite overwhelming in most cases. The gap between the data scientist and software engineer can be bridged by aiding a data scientist with the necessary software skills to deploy their machine learning model. This is where amazon sagemaker comes in very handy. With SageMaker, data scientists and developers can quickly and easily build and train machine learning models and directly deploy them into a production-ready hosted environment.

## Data
The dataset contains food reviews extracted from different review sections. It has various attributes but only the review feature will be used to train the model.

_Data is not included in this repository._

## Approach
- Data Loading
- Data Preprocessing

○ Data cleaning ○ Creating a sequence of data ○ Tokenization

- Model Building and Training ○ LSTM model building in PyTorch
- Model Deployment on Amazon Sagemaker

Modular Code Overview

Once you unzip the textgenerator_code.zip file, you can find the following folders within it.
1. Input
2. MLPipeline
3. NoteBook
4. Output
5. Sagemaker_Deployment
6. Engine.py
7. Readme.md
8. requirements.txt
1. The Input folder contains the data that we have for analysis. In our case, it includes reviews of the product
2. The Notebook folder contains the jupyter notebook file of the project
3. The ML_pipeline is a folder that contains all the functions put into different python files, which are appropriately named. These python functions are then called inside the Engine.py file
4. The Output folder contains the saved model
5. Sagemaker_Deployment folder contains the files for deployment
6. The requirements.txt file has all the required libraries with respective versions. Kindly install the file by using the command pip install -r requirements.txt
7. All the instructions for running the code are present in Readme.md file

## Tech stack
➔ Language: Python ➔ Libraries: pytorch, pandas, numpy, regex,boto3

## How to run
```bash
pip install -r sagemaker_code-updated/requirements.txt
```
Notebooks: [`Sage_Maker_Text_Generator.ipynb`](sagemaker_code-updated/NoteBook/Sage_Maker_Text_Generator.ipynb)

## Project structure
```
.gitignore
README.md
sagemaker_code-updated/
  Engine.py
  MLPipeline/
    Data_Processing.py
    Model.py
    Predict.py
    Tokens.py
    Train.py
  NoteBook/
    Sage_Maker_Text_Generator.ipynb
  Readme.md
  Sagemaker_Deployment/
    textgenerator_py/
  requirements.txt
```

## Credits
Based on a ProjectPro guided project.
