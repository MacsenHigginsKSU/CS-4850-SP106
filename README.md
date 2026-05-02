!IMPORTANT!
To run and test model, enter the following instruction in your terminal: 
    pip install -r requirements.txt

Given a dataset from PJM Interconnection LLC documenting system-wide energy consumption along the Eastern United States from 1998 to 2018, we aim to develop a forecasting model using Long Short-Term Memory (LSTM) modeling that can accurately predict usage based only on date and time.

The finished website can be viewed under the deployments tab.

Here is the basic organization:

CS-4850-SP106/ 
├── .gitignore			    | file in a Git repository that instructs Git which files to ignore 
├── README.md		        | contains relevant background and instructions for the project 
├── TensorFlow.ipynb	    | where the data was cleaned and the model was trained 
├── assets/			        | folder containing assets for the website deployment 
│   ├── images/ 
│   │   ├── KSU-Logo.jpg 
│   │   ├── KSU_ccse_logo.png 
│   │   ├── ksu-logo2.png 
│   │   ├── sp_jacob.png 
│   │   └── sp_macsen.png 
│   ├── macsen_resume.pdf 
│   ├── mystyles.css		| css file to maintain a consistent style of our website 
│   └── plot_2010.html		| using plotly, embedded an interactable graph to visualize the data 
├── demo.html			    | html code for the demo page 
├── electricity-data/		| our data can be sourced from this folder, sourced via Kaggle 
│   ├── AEP_hourly.csv 
│   ├── COMED_hourly.csv 
│   ├── DAYTON_hourly.csv 
│   ├── DEOK_hourly.csv 
│   ├── DOM_hourly.csv 
│   ├── DUQ_hourly.csv 
│   ├── EKPC_hourly.csv 
│   ├── FE_hourly.csv 
│   ├── NI_hourly.csv 
│   ├── PJME_hourly.csv 
│   ├── PJMW_hourly.csv 
│   ├── PJM_Load_hourly.csv 
│   ├── est_hourly.parquet 
│   └── pjm_hourly_est.csv 
├── index.html			    | html code for the landing page 
├── requirements.txt		| a file containing all dependencies needed to run the model code 
└── user_datetime_predictions.csv	| file we import to the demo that contains predictive data 