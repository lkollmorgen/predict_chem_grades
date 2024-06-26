# predict_chem_grades
### Laura Jones
### Last updated 5.22.2024
In this notebook, I explore a dataset collected from high school general chemistry students. The goal is to show students that minimal changes in their study habits, like studying for 1 more hour each week or ask more clarifying questions, will improve their grades in chemistry.<br>
Initially, a linear regression was applied through SKLearn, but later, the project was further developed using Tensorflow's Keras API.

### Most Recent Update
- Added new notebook, dataset 2 predictions
    - Changed keras model to wide, single-layer network


## Dataset Bias
This dataset was collected via Google Form, posted as an optional assinment on Google Classroom, so there is potential bias in which students decided to take the survey. Potentially, students with lower grades were not inclined to take the survey.<br>
In addition, the class is very lax and therefore, the class averages are very high.<br>
Finally, students could have been dishonest in their responses, potentially because they took the survey during class with peers present.

## Target Population and Sampled Population
This survey was offered to 89 general chemistry students in grades 10-12, with most being in 10th grade (15-17 years of age). The students attend a private school in southern california.<br>
Students have 4 classes per day and have 4 core classes(science, math, english, history), with the rest being electives.<br>
Dataset 1 was collected after students returned from winter break, so the grades are their semester 1 final grades.<br>
Dataset 2 summarizes the students' answers at the end of the 2nd semester, the final semester of the school year. 

## Data Exploration Bias
In the data exploration and analysis, extra attention is given to the students grades in relation to their hours studied, since I hope to encourage students to study more than 3 hours per week for general chemistry. 

## Initial Results Using SKLearn
- Lowest MAE for linear regression model was 5.17 (dataset 1) and 4.44 (dataset 2)
- Consistent results
The cross-validation scores for the Linear Regression are subpar. This is likely due to a lack of correlated features.<br>
Nonetheless, The final cells can be used to show students that, by asking clarifying questions and studying more, a student's grade can improve.

## Results using Tensorflow's Keras API
- Lowest MAE for deep learning model was 6.794 using a batch size of 10, 500 epochs, dropout of .3, and a wide model with two hidden layers at 1024 nodes each (dataset 1) and 5.875 using a batch size of 10, early stopping (around 200 epochs), dropout of .4, and a single, wide layer of 2048 nodes.
- Results changed drastically with minor changes in the batch size
- Results of model performance with varying hyperparameters are summarized below: <br>
![dataset 1 parameters table](images/dataset1_param_results.png "dataset1 parameters table")
- More exploration required for dataset 2

## Future Improvement
- PCA using dataset 2
- Attempt creating a single-layer, wide network for dataset 1

