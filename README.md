# finalproject_24

# Comparison of Transformer-based Sentiment Analysis Models
## Ivan Bibat
This is the Project Development repository for the final year research project. In this repository, the code for the scraping, pre-processing and sentiment classification of the specified dataset may be found, alongside the transformer-based sentiment analysis models trained and tested using the processed dataset. The goal for the project is to analyse and evaluate different transformer-based pre-trained sentiment analysis models with the retrieved data, then evaluate and compare the metrics of these models.

## Guide
Python 3.12
Anaconda Environment
PyTorch

twitter-roberta-base-sentiment, BERT-base-uncased, and distilBERT-base-uncased are the three transformer-based models used for training and evaluation in this project.
roBERTa model: https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment
BERT model: https://huggingface.co/google-bert/bert-base-uncased
distilBERT model: https://huggingface.co/distilbert/distilbert-base-uncased

The requirements.txt file allows for the installation of the required dependencies for the project. The following code will install the dependencies by typing the following into the Anaconda Prompt:
pip install -r requirements.txt

### Data Scraping
The data used in this project is retrieved by running the scraper.py file with the filter 'iPhone 15', identifying Reddit posts containing the keyword 'iPhone 15'. These entries are then appended into a .csv file.

The dataset is then put through preprocessing.ipynb, then through augmentation.ipynb, which performs preprocessing, cleaning and augmentation of the dataset. The data is outputted into a .csv file that is then put through into VADER.ipynb, which performs classification.


### Model Training
Each model takes in the cleaned, augmented, and labelled dataset, which is split into 3 subsets: training, validation, subset. These subsets are then used to train the model, validate the training, and then testing the model.
