# medical-provider-fraud-detection

## Setting Up the Environment 

1. Create the environment with `conda env create -f environment.yml`. The first line of the document sets the name of the environment, which is **medicalfraud**.

2. Activate the environment with `conda activate medicalfraud`.

## Instructions to Access Data 

The datasets used for this project can be found on Google Drive. Follow the instructions to upload the data.

1. Clone the repository on your local machine.
2. Download the datasets.
3. Open the repository and create a folder in the directory called *data*.
4. Upload the datasets to the *data* folder.

Link to dataset: https://drive.google.com/drive/folders/1lzkKIlauNlE3PLHl23IqdTR4gSp0t26X?usp=share_link

## Dataset Description

1. `Outpatientdata.csv` - Claim information for patients who visit the hospital, but do not stay at the hospital.
2. `Inpatientdata.csv` - Claim information for patients who stay at the hospital.

Features in datasets 1 and 2 include claim start and end dates, claim diagnoses codes, claim procedure codes, operating and attending physicians IDs, deductible amounts paid, and insurance reimbursement amounts.

3. `Beneficiarydata.csv` - Demographics of patients including gender, race, state, and chronic disease indicators. 
4. `Labels.csv` - Fraud and non fraud labels for provider IDs. 

In Analysis.ipynb, the datasets are joined to `df_full`, which will be saved in the *data* folder as `df_full.csv`. The granularity of the joined data is per patient, per provider, and per claim ID. 


## Reproducing Figures

Analysis.ipynb creates a *figures* folder. The argument save_fig is set to True and the figures will be saved to the folder when you create them. Change save_fig to False if you do not want to save the figures.