# Sentiment-Analysis-Quote-Output

## Preface
This is a part of the project that I did to close my master in Big Data and Data Science.

Please consider that I had zero experience when I developed it. Therefore, you will most probably find mistakes and bad practises.

For visualization support, please refer to the wiki section after reading this Readme file.

## Description
There is an initial database with approximately 500k labeled quotes and its authors. The labels depend on the quote content and they express the emotions of it: love, fear, hope, etc. Some quotes are multilabeled.

A model is created from the database. Different algorithms have been 
- Stocastic Gradient Descent (SGD)
- Support Vector Classification (SVC)
- Logistic Regression
- Lonf-short Term Memory (LSTM)

This selection has been based on research and best practises found online. The chosen final model has been the Neural Network (LTSM).


The idea is that the user introduces his state of mind at a certain moment in time. Specially when the user feels bad for some reason. Examples:

- "I feel kind of down because my boss did not respect my opinion in front of the others."
- "My girlfriend ridiculed me."
- "My father did not show me how to defend myself and now I have insecurities."

The model is going to classify the user's input and output a proper quote.

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
