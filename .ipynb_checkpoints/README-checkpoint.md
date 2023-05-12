# HealthBot

This project explored illness classification with symptom extraction to provide a more seamless interface.

For the illness classification training, these model-dataset pairs were used:

1. Decision Tree on Dataset 1
2. AutoModelForQuestionAnswering on Dataset 2

### Source 1

This dataset was used for the model in the 'main.py' script. It can be downloaded through this link:
```
https://www.kaggle.com/datasets/kaushil268/disease-prediction-using-machine-learning
```
### Source 2

This dataset consisted of medical conversations between an expert and a patient. The link to download this dataset is provided here:
```
https://github.com/abachaa/MedQuAD
```

# Source 3

MIMIC-III is a very large general medical dataset that the team came across later in the project cycle. Due to the format of the dataset, the team could not figure out a way extract the related data for illness classification.
The dataset can be downloaded from this link after the user has been certified and authorized to:
```
https://physionet.org/content/mimiciii/1.4/
```

## Directory Structure
```
|_ Dataset_Tests/
        |_ Dataset_1/
            |_ data/
                |_ Training.csv
                |_ Testing.csv
            |_ models/
                [ pre-trained models ]
                |_ DecisionTree.joblib
            |_ Model_Trained_SG.ipynb
            |_ Model_Trained_RK.ipynb
            |_ Model_SymExtract.ipynb
        |_ Dataset_2/
            |_ data/
                [ XML Files from the QA Dataset ]
            |_ XMLTraining.ipynb
|_ Keyword Extraction/
        |_ KeyBERT.ipynb
        |_ POS.ipynb
        |_ TF-IDF.ipynb
|_ main.py [ GUI code that loads pretraned model from Dataset 1 ]
```

## Usage and Demo

```
pip install -r requirements.txt
```

To run the GUI, run the 'main.py' script on your terminal with the following command:
```
python main.py
```

This will host a local and online GUI for you to go to by copy-pasting the web address it provides in the terminal.