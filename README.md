# Neural_Network_Charity_Analysis

## **Overview**
From our previous work with Beks on machine learning and neural networks, we are tasked to create a binary classifier that is capable  of predicting whether applicants will be successful if funded by Alphabet Soup.

## **Resources**
Software: Python 3.10.1, Google Colaboratories, Pandas 1.2.4, Jupyter Notebook 6.4.8
charity_data.csv

## **Results**
### *Data Preprocessing*
- What variable(s) are considered the target(s) for your model?
  Checking to see if the target is marked as successful in the DataFrame, indicating that it has been successfully funded by AlphabetSoup.
- What variable(s) are considered to be the features for your model?
  The IS_SUCCESSFUL column is the feature chosen for this dataset.
- What variable(s) are neither targets nor features, and should be removed from the input data?
  The EIN and NAME columns will not increase the accuracy of the model and can be removed to improve code efficiency.

### *Compiling, Training, and Evaluating the Model*
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  Was able to use three layers with 80 and 20 neurons with relu activation.  The final Output layer utilized sigmoid for the best result.
- Were you able to achieve the target model performance?
  Yes I was able to acheive 79.2% accuracy which is greater than the target model performance of 75%
- What steps did you take to try and increase model performance?
  The biggest impact of change was adding back the column Name that was previously excluded from the original model.  Then had to trim the number of     instances for the program to run without crashing.


## **Summary**
The overall results of the deep learning model, was we were able to achieve a respectable 79.2% accuracy on our model, by including the Name column of our csv dataset.  This increased our amount of data and had to be trimmed to allow Google Colabs to process.  By doing this, and changing our hidden layers to relu on all but the final output helped to achieve this.
To reduce the workload and perhaps saving adding Name back to the dataset, we could use the Random Forest Clarifier as it is less influenced by outliers in the dataset.
