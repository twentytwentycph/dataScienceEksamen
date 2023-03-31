README

Fake News Project
NDAB21002U Data Science (DS)

Credits:
Mateo Anusic | djz709 | djz709@alumni.ku.dk
Emil Thorlund | gpv679 | gpv679@alumni.ku.dk
Lucas A. Rosing | qgc922 | qgc922@alumni.ku.dk
Victor V. Bergien | tcg780 | tcg780@alumni.ku.dk

Introduction: 
This project is a group project for the NDAB21002U Data Science (DS) class of 2023, at the University of Copenhagen.
The aim of the project is to detect fake news using various text analysis and classification techniques.
The project is split into several Jupyter notebooks, namely Part 1 to Part 4.
Though, there are few sub notebooks usedfor the creation of the pipeline.

Dependencies:
To use this project, you'll need to install the following Python libraries:

nltk
cleantext
requests
dask
dask_ml
numpy
pandas
scikit-learn
imbalanced-learn
matplotlib
seaborn
pickle

Additionally, in order to execute the code, you must have downloaded the FakeNewsCorpus
from: https://github.com/several27/FakeNewsCorpus/releases/tag/v1.0.
The files downloaded from the previous link are split into nine compressed files.
Which require a multi-part decompression tool such as 7z to extract.
You will also need the LIAR dataset, from: https://www.cs.ucsb.edu/~william/data/liar_dataset.zip
Please note that in order to run the provided jupyter notebooks, you must alter line 12:
data = pd.read_csv('raw_shuffle_data_4GB.csv') in Part_1_pre.ipynb
To accept the entire uncompressed FakeNewsCorpus dataset as a csv file.
This is done by replacing line 12 with:
data = pd.read_csv('news_cleaned_2018_02_13.csv')
Futhermore, as the FakeNewsCorpus dataset is 29.322.513.705 bytes you may
encounter issue as the dataset may be larger than your systems memory.
This is why raw_shuffle_data_4GB.csv was chosen to be worked on, as it is a shuffled subset
of the FakeNewsCorpus dataset.

Installation:
You can install the required libraries using pip by running the following command:

pip install nltk cleantext requests dask dask_ml numpy pandas scikit-learn imbalanced-learn matplotlib seaborn pickle5

Note
This README assumes that you have Python 3.x installed on your system. If you have Python 2.x installed, some libraries may not be compatible,
and you may need to upgrade to Python 3.x or use a virtual environment.
