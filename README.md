# Natural Language Processing Exam - 02-01-2026
  **Malene Jensen**: Repository for Natural Language Processing Course at Master's of Cognitive Science

This repository contains code used for preprocessing, extraction of features, and classification analysis of child speech data.

The study aims to compare two groups of children, namely ASD and TD. In the project, I evaluate psycholinguistic features and sentence embeddings (Sentence-BERT) and their ability to dinstinguish between the aforementioned groups. 

## Structure of Repository

```
├── notebooks/
│ ├── preprocessing_and_parsing.ipynb
│ └── analysis_and_classifier.ipynb
├── requirements.txt
├── setup.sh
└── README.md
```


## Setup - Before running the code

First, you set your working directory to your current work folder, attaining the structure described above. 

Run the following in the terminal:
```
bash setup.sh
```

This will ensure all packages are installed from the requirements.txt file. 

To activate your newly made virtual environment, run the following code:
```
source .venv/bin/activate
```

You should now be able to select a kernel using the predefined packages from the requirements.txt file. 


## Notebooks
**preprocessing_and_parsing.ipynb**

In this notebook, I load and parse the CHAT transcripts, along with extracting features from filenames and headers. Furthermore, the initial preprocessing takes place here, which includes the calculation of certain features and outputting of dataframes used in the analysis. 


**analysis_and_classifier.ipynb**

In this notebook, I anonymize the data, visualize structures of the data, and analyze the data using classifiers:
- SBERT embedding classifier
- Psycholinguistic features classifier

## Data

Due to the high sensitivity of the data used in the study, it will not be uploaded to this repository. 

## Reproducibility

- Random seeds are fixed where applicable

- Group-based splitting ensures participants appear in only one data split

- All results reported in the accompanying paper are based on the held-out test set


## Ethical Considerations

This code is intended for research purposes only. The classification models produced are not diagnostic tools and should not be used for clinical decision-making. All analyses were conducted on anonymized data.





