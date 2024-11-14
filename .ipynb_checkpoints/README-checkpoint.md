# Project Overview

This project aims to classify the type of pitch thrown by a baseball pitcher using a machine learning model. By leveraging pitch-tracking data, including speed, spin rate, and break metrics, the goal is to accurately predict the pitch type (e.g., fastball, curveball, slider, etc.). This can provide insights for teams, coaches, and analysts looking to optimize game strategies or evaluate pitcher performance.

## Project steps

* Collected and preprocessed pitch-tracking data, focusing on metrics such as pitch speed, spin rate, and break
* Cleaned the dataset (handled null values, removed rarely used pitch types like knuckleballs)
* Generated features, including handedness of the pitcher, to capture variations in pitch profiles
* Visualized data distributions and relationships to gain insights into feature importance
* Built a predictive classification model to classify pitch types
* Leveraged Optuna to improve the model
* Evaluated model performance and explored areas for improvement

## Code

You can find all of the code necessary for the project [here]

Files:

* 'pitching_preds.ipynb' - the Jupyter notebook that contains all of the code, data exploration, and model-building process

# Local Setup

## Installation

The following need to be installed locally in order to explore the project:

* Python
* JupyterLab
* Python packages:
    * pandas
    * numpy
    * matplotlib
    * seaborn
    * scikit-learn

# Takeaways and Next Steps

## Results

* The model effectively classified common pitch types (e.g., fastball, slider) using speed, spin rate, and break metrics, with better accuracy observed for pitches that have distinct break profiles
* Handedness (is_lefty) helped differentiate pitch movement but had limited impact due to class imbalance
* High spin rate pitches, such as sliders and curveballs, were easier to classify, while pitches with overlapping speeds (e.g., fastballs and sliders) posed a challenge

## Next steps
*  Introduce additional features like release extension, effective speed, and game context (e.g., inning, pitch count) to improve model accuracy
* Incorporate data from previous seasons or minor league games to enhance model robustness, especially for underrepresented pitch types and left-handed pitchers

_More detailed takeaways and next steps can be found at the end of the Jupyter Notebook_