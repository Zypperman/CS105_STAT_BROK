# Final thoughts

Frankly, I wish I had a better way of working with you guys. The changes made in this commit were things that we coulda caught before submission but didn't, because QA wasn't done. I take proportionate blame given I submitted this version of the document at 6pm, 6 hours prior to submission. I was tired, and I finally had a working version of the code, and I hadn't realised the numerous errors that were made ie:

- descriptions not matching what was done, ie the yeo-johnson transformation failing to create a normal distribution. we shoulda just used the log transformation, since we were just creating features for the sake of exploration. Weak justification was also not fixed despite it being flagged.

- loose descriptions that don't match with code, ie correlation value thresholds between our predictors and response value, and our predictors themselves.

- code implementation errors, like how the train_test_split function was incorrectly splitting resulting in our model only training on 20% data and testing with 80% of the data, or that I was printing the coefficients used by model 1 for all 3 model evaluation segments, or that I had incorrectly stated that we were measuring the RMSE or MAE relative to the average of the prediction values instead of the mean.
    - side note, fortunately this did not impact our results significantly since arguably, if you trained on 20% of the data and still managed to get an acceptable accuracy testing with 80% of the data, the model would still be considered robust. the other implementation mistakes are also arguably negligible.

# Anyways, whats passed has passed.  
  好马不吃回头草. Lets just compensate and get full marks for the finals.

