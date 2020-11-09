# Sentiment-Analysis-Quote-Output

## Preface
This is a part of the project that I did to close my master in Big Data and Data Science. It represents an scenario where a supposed client is hiring me for a data science job.

Please consider that I had zero experience when I developed it. Therefore, you might find mistakes and bad practises.

IMPORTANT: For visualization support, please refer to the wiki section after reading this Readme file.


## Description
The client wants to create a model capable of clasify user sentiments. 

The user introduces his state of mind (written inputs) at a certain moment in time. Specially when the user feels bad for some reason. Examples:

- "I feel kind of down because my boss did not respect my opinion in front of the others."
- "My girlfriend ridiculed me."
- "My father did not show me how to defend myself and now I have insecurities."

The model is going to properly classif the user's inputs.

To train the model,t here is an initial dataset with approximately 500k labeled quotes and its authors. The labels depend on the quote content and they express the emotions of it: love, fear, hope, etc. Some quotes are multilabeled.

Different algorithms have been used:
- Stocastic Gradient Descent (SGD)
- Support Vector Classification (SVC)
- Logistic Regression
- Lonf-short Term Memory (LSTM)

This selection has been based on research and best practises found online. The chosen final model has been the Neural Network (LTSM).

The client also wants to increase the original dataset. He wants to extract tweets from twitter accounts which are posting daily quotes. For that, he asks to create a database in MongoDB where the original dataset with the 500k and the daily extracted tweets are kept.

The whole project has been carried out following CRISP-DM methodology (to solve for data mining). Therefore the there is a notebook for each phase:
- Phase 0: Data Understanding
- Phase 1: Business Understanding (no notebook)
- Phase 2: Data Understanding
- Phase 3: Data Preparation (tweet clean and extraction)
- Phase 4: Modeling (Supervised Learning)
- Phase 5: Evaluation
- Phase 6: Deployment

Any comment is always welcome!

## Table of Contents:
Not needed


## Installation:
No instalation possible


## Usage:
Perfectly explained inside the code


## Contributing: 
It would be appreciate to see how you would approach the project for better results. Please see the conclusions I gathered in the next section. The limitation of the data makes not possible to drastically improve the results.


## Conclusions: 
- With neural  network 41,1% reached. At some point, NN simplicity did not reduce overfitting. No more data available. Possibility to relabel. For instance bringing "death" and "fear" together under "death".
- There was scarcity in documentation to classify a multi-label problem.
- RNN bottleneck is that it is sequential processing of text → BERT could deliver better results (Minaee et al. 2020)
- I did not properly analyze the dataset at the beginning of the problem and that pushed me to delete many raws. If I had done that, I could have relabed some of the quotes and therefore get a better outcome.


## License:
No licenses.
