# IMDB-Reviews-Classification
Creating a AWD-LSTM based classifier for classifying movie reviews from the IMDB dataset

Library used: **Fastai** (1.0.60)

We have first trained a **Language Model** using the entire IMDB dataset, and set aside 15% (randomly chosen) of all the text files in the 'train','test' and 'unsup' folders as the validation set for this purpose.
We then used the **encoder** of this language model to create and train a **Classifier** that predicts the classes ['pos'/'neg'] of each movie review.

The following trained models can be found [here on Google Drive](https://drive.google.com/drive/folders/1RenHK2Jhuvw-J1stoxjeULbQS_c70C76?usp=sharing)

**final_trained_language_model.pkl**: Trained Language Model exported for inferences purposes.
**final_trained_language_classifier.pkl**: Trained Language Classifier exported for inferences purposes.

While finetuning the language classifier, we choose our learning rates from the learning rate finder, and we divided the first part of the slice with a factor (**2.6^4**) based on the [ULMFiT paper](https://arxiv.org/abs/1801.06146) written by **Jeremy Howard** and **Sebastian Ruder**.