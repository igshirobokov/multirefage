MultiREFAGE is a web application for estimating biological age based on cranial suture closure.
It uses trained Random Forest Regressors and supports age prediction through a clean web interface. The name reflects its core idea: MULTIple REFerence AGE groups.


🔍 Project Highlights
Multiple reference models based on estimated age

Uses machine learning (Random Forest) to model cranial suture obliteration

Accepts input data as .xlsx files with cranial features and a "expected" age estimate

Outputs include:

Predicted age

95% confidence interval (based on LOOCV MAE)

Features
User-friendly web interface hosted on Render.com

Upload your data and get predictions instantly

View and download results in Excel format

Works fully online, no installation needed

File Format
The input Excel file must contain:

1. Optional ID column
2. Discrete traits based on the degree of suture obliteration (Meindl, Lovejoy, 1985) used by the model
3. Column "Expected_age" — a visual or estimated age (can be "50+", "40 50", "20" etc.)


A sample file is available: example.xlsx

How it works
You upload an Excel file with data

The app parses the expected age value to select the most appropriate reference model.

A Random Forest Regressor makes the prediction.

You get:

A downloadable .xlsx file with results

Confidence intervals based on LOOCV-derived MAE

🏛 Funding Acknowledgment
This project is supported by the Russian Science Foundation
Grant № 24-28-01050 "In search of effective methods for sex and age assessment based on the skull"

License
MIT License – free to use and modify for scientific or non-commercial purposes.
