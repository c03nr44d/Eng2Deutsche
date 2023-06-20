# Eng2German
English to german seq2seq machine translation model

The files provided are 3 separate notebooks and 3 datasets that have been preprocessed and split from the original dataset. We describe them here;

### Data_Handling.ipnyb 
describes our data preprocessing of the original English German dataset downloaded from Kaggle Bilingual Sentence Pairs, and exporting them into 3 CSVs, namely df_train.csv, df_test.csv, df_val.csv. We do this so that we can replicate the model’s performance.

### Model_Training.ipynb
describes our model training process, and exports the model as a h5 file for portability.

### Evaluation.ipynb 
evaluates our model and contains a custom translator for the user’s own input.

The latter 2 notebooks were run on Google Colab, for their GPU hardware accelerator, and saving the .h5 file on Google Drive. If you would like to run this locally, skip the mounting of the drive cell and carry on.

---
### Areas for improvement:
