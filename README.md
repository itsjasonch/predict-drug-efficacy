# predict-drug-efficacy
### **BIEN 3320 Group Project - Machine Learning-based Prediction of Drug Efficacy Targeting FEN1 for Cancer Therapy**

Targeting FEN1 has been verified as an effective strategy in mono or combined treatment of cancer. We will build machine learning models to predict the efficacy of potential drugs towards FEN1, using both regression and binary classificaiton approaches. 

Reference: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9312813/
<br/><br/><br/>
**Library & Software**

The entire project was developed using the Kaggle environment and included additional installation of RDKit (version 2023.3.1) and PubChemPy (version 1.0.4). PaDEL-descriptor software was downloaded from https://github.com/dataprofessor/bioinformatics.
<br/><br/><br/>
**Usage**

[1] Dataset

We have used the bioassay record (AID588795) of the assay project "qHTS Assay for the Inhibitors of Human FEN1” in PubChem to train our ML model. The raw bioassay data are available at https://pubchem.ncbi.nlm.nih.gov/bioassay/588795. For prediction, we have compiled a list of licensed cancer drugs from https://www.anticancerfund.org/en/cancerdrugs-db. All processed datasets are contained in "aid588795.zip".
<br/><br/>
[2] Code

analysis.ipynb  --- Exploratory data analysis

fp_reg.ipynb    --- Regression model using Morgan Fingerprint encoding

desc_reg.ipynb  --- Regression model using PaDEL-descriptor encoding

fp_clf.ipynb    --- Binary classification model using Morgan Fingerprint encoding, and performing prediction for the licensed cancer drugs

desc_clf.ipynb  --- Binary classification model using PaDEL-descriptor encoding
<br/><br/>
[2] Prediction

The names of the predicted positive cancer drugs were stored in "pred-positive-drugs.csv".
