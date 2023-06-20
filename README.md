# Eng2German
English to German seq2seq machine translation model, as part of our final project for WBAI059-05 Natural Language Processing at the University of Groningen (RUG).

The files provided are 3 separate notebooks and 3 datasets that have been preprocessed and split from the original dataset. We describe them here and they should be run in the following order;

### 1) Data_Handling.ipnyb 
describes our data preprocessing of the original English German dataset downloaded from Kaggle Bilingual Sentence Pairs, and exporting them into 3 CSVs, namely df_train.csv, df_test.csv, df_val.csv. We do this so that we can replicate the model’s performance. The files we obtained are also provided in our repository.

### 2) Model_Training.ipynb
describes our model training process, and exports the model as a h5 file for portability. We do not include the model as it 

### 3) Evaluation.ipynb 
evaluates our model and contains a custom translator for the user’s own input. requires the model (.h5 file) and the datasets to run.

The latter 2 notebooks were run on Google Colab, for their GPU hardware accelerator, and saving the .h5 file on Google Drive. If you would like to run this locally, skip the mounting of the drive cell and carry on.

---
### Setup steps and Dependencies:

Download the original dataset from Kaggle. We used the English German bilingual sentence pairs [dataset](https://www.kaggle.com/datasets/alincijov/bilingual-sentence-pairs), named deu.txt.
Have the required packages installed. You may follow ours at requirements.txt.

---
### Areas for improvement:
Our model could be improved in a number of ways. 

- Data.
We decided to train our model on sentences that have a maximum length of fifteen words. This causes the model to be less good at predicting sentences that have more than fifteen words. Therefore, our model could be improved by training it on a more diverse dataset, also including longer sentences (if you have enough computational power).

- Add attention mechanisms.
Currently, the model does not have any attention mechanism. Adding this could improve the model’s results in several ways, such as dealing with long sequences, improve interpretability, and improve the overall performance of the model.
- Adding more layers and tuning the hyperparameters better.
 We tried to tune the hyperparameters as best as possible, but there is probably still a lot of room for improvement.

---

### Useful Information:

The Metric for Evaluation of Translation with Explicit ORdering ([METEOR](https://www.cs.cmu.edu/~alavie/METEOR/pdf/Banerjee-Lavie-2005-METEOR.pdf)).

The Bi-Lingual Evaluation Understudy ([BLEU](https://aclanthology.org/P02-1040.pdf)) metric.
