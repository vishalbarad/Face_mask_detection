# Face_mask_detection
This project is a part of the CNN Deep learning.
Dataset https://drive.google.com/drive/folders/1P3gIgFUMbdl5tSqx1pK385bz4t0mxEvW?usp=sharing

#### -- Project Status: [Completed]

## Project Intro/Objective
The purpose of this project is to detect whether person has wear mask or not.

### Methods Used
* Data gathering
* Data preprocessing
* Build CNN model
* Model evaluation
* Predictive Modeling


### Technologies
* Python
* Numpy 
* Pandas
* jupyter
* joblib
* HTML
* CSS
* JavaScript
* Flask
* Heroku

## Project Description
This is project based on regression ml algorithm. If you know the venue, current over runs and wickets then you simply predict score by just providing the last 5 over runs and wickets.
Dataset used by this project is 'ipl.csv' downloaded from kaggle. After downloading and importing dataset(in jupyter Notebook) i did data cleaning first like dropping some unnecessary columns, handling missing values, performing one-hot encoding on categorical variables.
After that i just divided my dataset into dependent and independent features. (Independent features=Venue,runs,wickets,etc.. | Dependent feature=total)
After that i just dropped first 5 overs data in every match because first 5 overs are powerplay over ,so i just ignored it.
After that i split data into training data and testing data.
After that i perform model selection in which i chose 'Multiplelinear', 'Ridge', 'Lasso', 'Decision tree' and 'Random forest' regression algorithm and count accuracy score so i got

|Model          |Training_accuracy |Testing_accuracy |
|-------------- |----------------- |---------------- |
|Linera         |0.678325          |0.668358         |
|Ridge          |0.678321          |0.668351         |
|Lasso          |0.678321          |0.668347         |
|Decision-tree  |0.999963          |0.907869         |
|Random forest	|0.989497	         |0.949162         |

As we can saw among all regression Decision tree reg and Random forest regression gave the better result so we choose Random forest for predection beacause Ensemble based aglo does not overfit the data.
After that i saved model using 'joblib' library. After that I creted UI in flask and deployed on 'Heroku'.

## Needs of this project

- frontend developers
- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- writeup/reporting

## Contact
* Feel free to contact me any questions or if you are interested in contributing!


<h1 align=center>Thank You</h1>

