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
* jupyter
* Numpy 
* Matplotlib
* tensorflow>=2.1.0
* keras==2.3.1

## Project Description
This is project based on CNN model. 
Dataset used by this project is 'https://drive.google.com/drive/folders/1P3gIgFUMbdl5tSqx1pK385bz4t0mxEvW?usp=sharing'. Dataset conatins train, test and validation data in each there are two class 'with_mask' and 'without_mask'. After downloading and importing dataset(in Google colab) i did data image augmentation first like rescale image, rotate image, flip image, zoom image etc.
**Data Augmentation: It is a way to generate more training data frm our currenet set. It augments the training data by generating new eg via random transformation of existing ones. This way we artificially boost the size of the training set, reducing overfitting.**
After that i just use 'model checkpoint' callback function to save best model.
After that i just create CNN model as follow
<img src="https://github.com/vishalbarad/Face_mask_detection/blob/master/cnn_scratch.png">
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

