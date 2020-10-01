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

Cement (component 1) -- quantitative -- kg in a m3 mixture -- Input Variable
Blast Furnace Slag (component 2) -- quantitative -- kg in a m3 mixture -- Input Variable
Fly Ash (component 3) -- quantitative -- kg in a m3 mixture -- Input Variable
Water (component 4) -- quantitative -- kg in a m3 mixture -- Input Variable
Superplasticizer (component 5) -- quantitative -- kg in a m3 mixture -- Input Variable
Coarse Aggregate (component 6) -- quantitative -- kg in a m3 mixture -- Input Variable
Fine Aggregate (component 7) -- quantitative -- kg in a m3 mixture -- Input Variable
Age -- quantitative -- Day (1~365) -- Input Variable
