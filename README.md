# Predicting sales from advertising using linear regression 
Have you ever wondered how much of a product you would sell given the money you spent to advertise it? This machine learning model untilises a linear regression algorithm to predict how much sales a given product gets using information on how much was spent on its advertising. 

## Table of Contents 
- [Data Information](#data-information)
- [Technologies](#technologies)
- [Setup](#setup)
- [Model tutorial](#how-to-use-this-model-to-make-predictions-yourself) 

## Data Information 
The dataset used to train this machine learning model is Advertising.csv, which you can download [here](http://faculty.marshall.usc.edu/gareth-james/ISL/data.html) (it is also attached to this repository).  
- The dataset contains 200 observations. 
- The 3 features for this dataset are named 'TV', 'radio', and 'newspaper', representing the method of advertisement. The associated data with these features represent the amount of money (in thousands of dollars) spent on each method of advertisement. 
- The response label for this dataset is named 'sales', which represents the number the sales of a particular product that was advertised. The data assocated with this label represent the number of sales (in thousands of units sold) made for the particular product that was advertised.  

## Technologies
This project is created with: 
- Jupyter notebook 
- python 3.8 

## Dependencies 
Libraries and packages used in this project (also outlined in the environment.yaml file attached to this repository) 
- pandas 
- sci-kit learn 
- seaborn 
- jupyter 
- matplotlib 
- numpy 

## Setup 
Here are the outlined instuctions to run this project on your local device. (Note: I have used Conda in this setup instruction. You may use your own prefered package manager).   

First, clone this repository onto your local device by entering the line below into your terminal:  
`git clone https://github.com/R0YLUO/My-first-ML-project.git`

Then, you need to create an environment with the necessary dependencies. These dependencies are specified in the environment.yaml file attached to this repository, which you would have just cloned to your local device. So to create the environment, in your terminal, first change the directory to the cloned folder. Then run the following command:  
`conda env create --file environment.yaml --name myenv`

Now, you can activate the environment by entering the command `conda activate myenv` 

Finally, open jupyter notebook by entering the command `jupyter notebook` and you should be able to run the project locally. 

## How to use this model to make predictions yourself 
The model has been trained with the provided Advertising.csv dataset using a linear regression model. If you wish to try it out and predict sales using the model, add the following code to the notebook:  
`print(predict(<TV-AD-SPENDING>, <RADIO-AD-SPENDING>, <NEWSPAPER-AD-SPENDING>)` 
and replace `<TV-AD-SPENDING>`, `<RADIO-AD-SPENDING>`, `<NEWSPAPER-AD-SPENDING>` with the monetary values spent on each respective advertising, in thousands of dollars.
For example, if you enter the code `print(predict(100, 50, 50)`, you are predicting the number of sales of a particular product that you spent $100,000 on TV ads, $50,000 on radio ads, and $50,000 on newspaper ads. The output would be `16.89629275`, meaning the predicted number of sales for that product will be 16,896. 
