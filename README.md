# Credit_Risk_Analysis

## Overview
     The purpose of this analysis was to take the dataset and use different methods to sample the data.
Various methods to sample the data have been applied such as oversampling with the RandomOverSampler
and SMOTE. Additional methods such as undersampling with ClusterCentroids and the combinational approach
with the SMOTEEN method have also been applied to sample the data. Following the sampling, two machine
learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier, have been compared to
predict credit risk.

## Results
![NRO](https://user-images.githubusercontent.com/87545554/143496342-330d2634-53fc-4038-acc8-9d730a2b738d.jpg)
- The balanced accuracy score for the RandomOverSampler shows that the model was correct roughly
61% of the time
- The precision for low risk was 1.00 and the sensitivity was 0.70. This would mean that the model
did a fairly good job at predicting the data.
- The precision for high risk was 0.01 and the sensitivity was 0.51. This would mean that the model
found many false positivies for high risk and found roughly 50% of those who were actually high risk.

![smote](https://user-images.githubusercontent.com/87545554/143500574-fdc72a1a-c408-45f2-b453-334a7b73dbe4.jpg)
- The balanced accuracy score for the SMOTE model predicted correctly 65% of the time.
- The precision for low risk was 1.00 and sensitivity was 0.70. This is similar to the previous model.
- The precision for high risk was 0.01 and sensitivity was at 0.60. This would mean that there are
still just as many false positivites as the previous model, but did better at detecting more potential
high risks.

![undersampling](https://user-images.githubusercontent.com/87545554/143500708-879334a0-d947-4dfd-aab4-da2d203aeb5a.jpg)
- The balanced accuracy score for the undersmapling method found the model to be correct just over
50% of the time.
- The method found the precision for low risk to be 0.99 and sensitivity to be 0.43 which would
mean that the model did worse than the oversampling method.
- The precision for high risk was 0.01 and sensitivity to be 0.59. Overall the undersampling 
method did worse for both high and low risk compared to oversampling.

![smoteen](https://user-images.githubusercontent.com/87545554/143500810-df665b5d-c509-42bc-b2cc-e7488041c208.jpg)
- The balanced score for the combination method was 0.62.
- The precision for low risk was 1.00 and 0.57 for the sensitivity. This would show that the results
are fairly similar to the the first oversampling method.
- The precision for high risk was 0.01 and 0.68 for the sensitivity. The model's results are similar
to the first oversampling method.

![BRFC](https://user-images.githubusercontent.com/87545554/143501008-04d906d0-8df0-4f5e-aad3-94aa5c1e7442.jpg)
- The balanced accuracy score for the BRFC model was 0.89 which did significantly better than the
previous models.
- The high risk precision came to be 0.03 and sensitivty was 0.59. The model did better at finding more true
positives, but did not perform as well in terms of sensitivty to the oversampling method.
- The low risk precision was at 1.00 and sensitivty at 0.90. The model did really well at finding low risk.

![EEC](https://user-images.githubusercontent.com/87545554/144109404-88cc7679-411c-4bf9-8b1e-dd50265d4e21.jpg)
- The balanced accuracy score was 0.94 which is the best result that we've had out of all the models.
- The high risk precision came to be 0.08 and sensitivty was 0.89. The model has the best results for
finding high risk.
- The low risk was nearly perfect with a precision of 1.00 and a sensitivity of 0.95 meaning it nearly
correctly calculated all low risks.

## Summary
     The machine learning models did better than any of the sampling methods. However, out of all the
methods, the undersampling had the least favorable results while the EasyEnsembleMethod provided
the best results out of all the methods. Out of all the methods, the EasyEnsembleMethod mdoel would be the
most recommended the one. This would be because detection for low risk has both high precision and high
sensitivity. As for the high risk it can be noticed that it is more likely to detect true positives compared
to any of the other models tested with very little trade off on the sensitivity. 

