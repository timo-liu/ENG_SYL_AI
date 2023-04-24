# ENG_SYL_AI
GRU-based Neural Network designed for splitting English orthographies into syllables. The model was trained on data scraped from Google Dictionary search results(around 26,500 word entries). Data was hand-pruned and cleaned before training.

This repository contains the code for my English Syllabification model and data, as well as data on the model's performance over 10 trials(F1 scores, Brier scores, syllable accuracy, average Levenshtein edit distance, etc) as well as the performance of other contemporary syllabification algorithms over the same validation data(Hyphenate and syllables from PyPi).

Over 10 trials, ENG_SYL_AI achieved an average F1 score of 0.91(precision= 0.91, recall= 0.91), compared to Hyphenate's F1 score of 0.88(precision= .97, recall = 0.81).

## Plans for Improvement
A major failing of ENG_SYL_AI is that it struggles with syllabification of more complex words. In order to improve the model efficacy, an additional sub_word_tokenization model can be introduced before the syllabification module.

