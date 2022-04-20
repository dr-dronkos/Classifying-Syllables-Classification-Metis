# Syllable Classifier: Using supervised Machine Learning to predict whether a syllable is Gurung or Nepali

## Abstract
This project uses data from my doctoral dissertation (Ronkos 2020) to see whether a supervised Machine Learning model can be trained to correctly classify syllables as belonging to one of two languages -- Gurung, a Tibeto-Burman minority language of Nepal, or Nepali, an Indo-Aryan language that is the official langauge of Nepal. The data is coded differently for consonants and vowels; consonants are described using categorical features since the methods of acoustically measruing consonants vary greatly depending on the type of consonant (i.e. voice onset time for obstruents but formants for sonorants), while vowels are coded using acoustic data extracted from recorded soundfiles using the open source software Praat (Boersema & Weenik 2022). The soundfiles were recorded with the help of 5 speakers of Gurung and 5 speakers of Nepali using a Sennheiser ME66 microphone and a Zoom H4N recorder, and together comprise a fairly balanced dataset of 5,099 syllables (2,313 Gurung syllables and 2,786 Nepali syllables). Using Scikit Learn, I fit a baseline logistic regression model to see if it would perform better than chance. This initial model had an acccracy of 0.767. After some attempts at additional feature engineering did not increase performance, I ultimately fit a Stacking Ensemble model that combined K-Nearest Neighbors, Decision Tree, and Logistic Regression models to achieve an accuracy of 0.91. This suggests that coding syllables using the features linguistis have determined are useful in human speech perception may also be useful in machine learning classification of speech. Ths has applications in automatic speech recognition, accent or language detection, or other circumstances where it my be useful to detect a novel speaker's language using only syllable information rather than pretraining on entire words or lexicons.




The elictation sessions took place in 2017 in New York City, as well as Sikles Village and Kathmandu, Nepal.


