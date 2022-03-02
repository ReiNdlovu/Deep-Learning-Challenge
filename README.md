# Deep-Learning-Challenge

#### Data Preprocessing
----
1. What variable(s) are considered the target for your model?
Answer: The ear marked target for the model was the "Is-Successful" column and identifying if the money was utilized effectively; and it was.
---
2. What variable(s) are considered to be the features for your model?
Answer: The features considered and used are; Name, Application, Type, Affiliation, Classification, Use_Case, Organization, Income_AMT,Special_Considerations, Status, & Ask_AMT
---
3. What variable(s) are neither and should be removed from the input data? 
Answer: The employer identificaiton was dropped because the data set could have skewed the results.

Answer: SPECIAL_CONSIDERATIONS could be droped from the analyzed data given the small percentage of cases that had any special consideration. Also, not all special considerations cannot be quantified.

Answer: Status should be dropped because the values have no range and there don't serve any purpose on the data set.

#### Compiling, Training, and Evaluating the Model
---- 
1. How many neurons, layers, and and activation functions did you select for your neural network model, and why?
Answer: Three hidden layers each with many neurons were used as this improved efficiency by increasing the accuracy above 75%. The number of epochs remained the same. Activation function #1 was 'relu', and the 2nd and 3rd were 'sigmoid'and the output function was 'sigmoid'. To the betterment of the model changing the 2nd and 3rd activation functions to 'sigmoid' also helped improve the accuracy. 
---
2. Were you able to achieve the target model performance?
Answer: Yes!
---
3. What steps did you take to try and increase model performance?
Answer: I converted the 'NAME' column into data points which had the biggest impact on improving efficiency. Also, the model additionally required addition of a third layer and using the "sigmoid" activation function for the 2nd and 3rd layer.

#### Summary
----
Altogether, by increasing the accuracy over 75% we were able to correctly classify each of the points in the test dataset 75% of the time. In addition, the applicants had a 80% chance of being successful if they had the following:
- The NAME of the applicant appears more than 5 times (they have applied more than 5 times)
- The type of APPLICATION is one of the following; T3, T4, T5, T6, T7, T8, T10, and T19
- The application has the following CLASSIFICATION; C1000, C2000, C3000, C1200, and C2100.

The recommended model would be the Random Forest model because Random Forest are good for classification problems due no scaling needed to be done. Using this model would produce a 78% accuracy. 
