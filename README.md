# IMDB-Reviews-Classification
Creating a AWD-LSTM based classifier for classifying movie reviews from the IMDB dataset

Library used: **Fastai**

We have first trained a **Language Model** using the entire IMDB dataset, and set aside 15% (randomly chosen) of all the text files in the 'train','test' and 'unsup' folders as the validation set for this purpose.
We then used the **encoder** of this language model to create and train a **Classifier** that predicts the classes ['pos'/'neg'] of each movie review.

**final_trained_language_model.pkl**: Trained Language Model exported for inferences purposes.
**final_trained_language_classifier.pkl**: Trained Language Classifier exported for inferences purposes.
