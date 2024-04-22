# predict_chem_grades
### Laura Jones
### Last updated 4.22.2024
In this notebook, I explore a dataset collected from high school general chemistry students. The goal is to show students that minimal changes in their study habits, like studying for 1 more hour each week or ask more clarifying questions, will improve their grades in chemistry.

## Dataset Bias
This dataset was collected via Google Form, posted as an optional assinment on Google Classroom, so there is potential bias in which students decided to take the survey. Potentially, students with lower grades were not inclined to take the survey.<br>
In addition, the class is very lax and therefore, the class averages are very high.<br>
Finally, students could have been dishonest in their responses, potentially because they took the survey during class with peers present.

## Target Population and Sampled Population
This survey was offered to 89 general chemistry students in grades 10-12, with most being in 10th grade (15-17 years of age). The students attend a private school in southern california.<br>
Students have 4 classes per day and have 4 core classes(science, math, english, history), with the rest being electives.<br>
The data was collected after students returned from winter break, so the grades are their semester 1 final grades.

## Data Exploration Bias
In the dta exploration and analysis, extra attention is given to the students grades in relation to their hours studied, since I hope to encourage students to study more than 3 hours per week for general chemistry. 

## Results
The cross-validation scores for the Linear Regression and Decision Tree models are subpar. This is likely due to a lack of correlated features.<br>
Nonetheless, The final cells can be used to show students that, by asking clarifying questions and studying more, a student's grade can improve.

## Future Improvement
- Collecting more features, such as 'study methods', 'attendance', 'effort during warmup activities', 'hours spent in extracurriculars', and the like
- Encouraging honesty in survey responses
- Mandatory survey response
- Trying other models