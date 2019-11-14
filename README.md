# Predict Abelone Age from Given Features

This study creates a regressor to predict abalone (fish) age given several features.

The features are:

sex, 
length
diameter
height
whole_weight
shucked_weight
viscera_weight
shell_weight

Target:

rings (+ 1.5) = age in years

Determining abalone age is manually intensive.  Conservationists need to cut into the fish and determine how many fat rings are present.  Modeling aleviates this issue.

The data set can be found at this link: https://archive.ics.uci.edu/ml/datasets/Abalone

In the code file I perform a range of basic EDA on the data set.  I subsequently baseline test a range of GLMs, non-parametric models, and ensemble models to determine which work best on the training data using 10 fold CV.

I then scale the data and again evaluate models using 10 fold CV.

I select the best model (several are close) and tune hyper parameters using a grid-search.

Lastly, I finalize the model and test performance on a validation set.


