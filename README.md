# Concrete Compressive Strength prediction

# Contents
- Demo
- Dataset Information
- Installation
- Technical Aspect
- Write Flask App
- Procfile
- Create requirements.txt 
- Deployment in local machine using Flask
- Deployment of machine learning model in Heroku using Flask


# Demo

https://compressive.herokuapp.com/

# Dataset Information

Problem Statement
To build a regression model to predict the concrete compressive strength based on the different features in the training data. 

Name -- Data Type -- Measurement -- Description

- Cement (component 1) -- quantitative -- kg in a m3 mixture -- Input Variable
- Blast Furnace Slag (component 2) -- quantitative -- kg in a m3 mixture -- Input Variable
- Fly Ash (component 3) -- quantitative -- kg in a m3 mixture -- Input Variable
- Water (component 4) -- quantitative -- kg in a m3 mixture -- Input Variable
- Superplasticizer (component 5) -- quantitative -- kg in a m3 mixture -- Input Variable
- Coarse Aggregate (component 6) -- quantitative -- kg in a m3 mixture -- Input Variable
- Fine Aggregate (component 7) -- quantitative -- kg in a m3 mixture -- Input Variable
- Age -- quantitative -- Day (1~365) -- Input Variable


# Technical Aspect

Content
```diff
1)Data Cleaning
1.1) Finding Out missing values
1.1) Finding Outliers and adjusting outliers
2) Data Exploration
3) Feature Engineering - Gaussian Transformation
4) Feature Selection
5) Algorithm
```

# Installation

To install the required packages and libraries, run this command in the project directory after cloning the repository:
```diff
pip install -r requirements.txt
```

- Create and Pickle a Machine Learning Model
```diff
import pickle
pickle.dump(model, open(‘model.pkl’, ‘wb’))
```

# Write Flask App

Open up your jupyter notebook and create a new .py file inside the working directory named app.py

The structure of the code follows:

```diff
Load pickled model
Name Flask app
Create route predict
Create Template
```

# Procfile
A Procfile specifies the commands that are executed by a Heroku app on startup. To create one, open up a new file named Procfile (no extension) in the working directory and paste the following. Flask command to run our app

```diff
  web: gunicorn app:app
```

# Create requirements.txt
```diff
The requirements.txt file will contain all of the dependencies for the flask app. To create a requirements.txt, run the following in your terminal from the working directory:
```

# Deployment in local machine using Streamlit

```diff
python run -- app.py
```

# Deployment of machine learning model in Heroku using Flask


1) First Create app name
2) Make sure it is connected to GitHub
<img src='photos/github.png' width="700" height="400">
3) Then click press on Deploy

