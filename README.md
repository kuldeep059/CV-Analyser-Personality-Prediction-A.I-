# ARTIFICIAL INTELLIGENCE PROJECT 

## Personality Prediction System

### Objective
This system predicts a person's personality based on their resume using OCEAN values (Openness, Conscientiousness, Extraversion, Agreeableness, Neuroticism). It aids in selecting the right candidate for jobs, reducing the workload of HR departments.

### Big Five Personality Traits
1. **Openness**: Creativity and desire for new experiences.
2. **Conscientiousness**: Organization and thoroughness.
3. **Extraversion/Introversion**: Sociability and energy from crowds.
4. **Agreeableness**: Getting along with others.
5. **Natural Reactions**: Emotional stability and response to stress.

### Dependencies
- os
- pandas
- numpy
- tkinter
- functools
- pyresparser
- sklearn
- nltk
- spaCy

### System Description

1. **train_model class**
   - **train method**: Reads data from a CSV file, trains a logistic regression model using 7 values (gender, age, 5 personality traits).
   - **test method**: Predicts personality using an array of values.

2. **main method**
   - Creates a train_model object, trains the model.
   - Designs the landing page using tkinter with a "Predict Personality" button.

3. **predict_person method**
   - Opens a new window for user input.
   - Labels and entries for input fields.
   - "Choose File" button for resume selection calls the OpenFile method.
   - Submit button passes values to prediction_result.

4. **OpenFile method**
   - Opens directory for file selection.
   - Updates button name with the chosen file.

5. **prediction_result method**
   - Closes previous window, calls test method, stores results.
   - Parses resume information.
   - Displays parsed information and predicted personality traits in a full-screen window.
