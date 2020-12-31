# SyriaTel Customer Analysis

## Introduction/Methodology
In this project, I seeked to provide SyriaTel, a telecommunications company, solutions regarding customer retention. Before diving into the models, the approach was an important part of what led to my conclusions. In our dataset, there were a variety of factors I observed, and one of the aims was to determine the most important variables while determining if a customer would continue using SyriaTel's services. In other words, identifying the areas where SyriaTel has the most room for improvement was a key focus. This way, I would be able to determine the factors that were most helpful and most costly to SyriaTel.
For each model, we also observed a 2x2 confusion matrix as well as four metrics (accuracy, recall, precision, and F1). The confusion matrices are an easy way to visualize the accuracy of each model. Numbers in the top-left and bottom-right corners represent correct predictions, while the other corners represent incorrect predictions. Accuracy is all about the percentage of predictions (whether or not a customer churned) that were correct. That is a very important metric, but F1 was also a key emphasis, as it considers both precision and recall. Therefore, a high F1 score generally indicates a model that is reliable all-around.

## Preliminary Models
The first model, which was used only as a preliminary step before diving into models with a higher chance of being appropriate, was a linear regression (in this case, the dependent variable only has two outcomes, so a linear regression does not have a good chance of being a good fit). One of the takeaways was that a couple of fields (account length and area code) were better removed than kept in. The data in these columns appeared to be clearly statistically insignificant, and any correlation with the dependent variable would not be spurious. Another takeaway from the linear regression and subsequent steps were that some columns were unnecessary and should be removed due to strong multicollinearity (five pairs of variables had correlations above .95; no others were above .65). The next model was the logistic regression. Having identified multicollinearity, the next step was to deal with the class imbalance. Early on, it was easy to identify a class imbalance, as only 14% of customers in the dataset churned to another company. Through the use of SMOTE, I created synthetic data to populate the minority class ("churn" class) to make it a 50-50 split. That improved the confusion matrix (previously, all predictions had been for "churn," despite it being the minority class), but the metrics still left much to be desired (.69 accuracy, .40 F1).

## Intermediate Models
The next attempt was a K Nearest Neighbors model. This is a regression algorithm that uses nearby points for predictions. Optimizing this model involved finding the value of k (a constant) where the best fit is. In this case, k is optimized with a value of 7.

## Final Model


## Conclusion/Recommendations
