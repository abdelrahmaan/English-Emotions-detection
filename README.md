# English-Emotions-detection

I gathered three datasets from Kaggle for modeling.

1- Emotion Detection from Text.

2- Emotion Dataset for Emotion Recognition Tasks.

3- Emotions dataset for NLP.

After that, I found the data is unblanced, so i made a data augmentation for minority labels by `DistalBERT` word embedding.

Afterward doing text preprocessing like removing emojis, removing links, removing mentions, removing hashtags, removing Punctuations,

removing duplicate characters, removing the new lines, just keep the English language.

At the end apply the modeling on two-phase:

1- `Original` data "Unbalanced data" by `DistalBERT` model with 49604 row data, and got around `0.76 F1-macro avg` on testing data, and it took 1.5H.

2- `Augmented` data "balanced data" by `DistalBERT` model with 74944 row data, and got around `0.85 F1-macro avg` on testing data, and it took 2.5H.


