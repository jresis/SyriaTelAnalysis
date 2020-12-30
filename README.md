# SyriaTel Customer Analysis

## Introduction/Methodology
In this project, I seeked to provide SyriaTel, a telecommunications company, solutions regarding customer retention. Before diving into the models, the approach was an important part of what led to my conclusions. In our dataset, there were a variety of factors I observed, and one of the aims was to determine the most important variables while determining if a customer would continue using SyriaTel's services. In other words, identifying the areas where SyriaTel has the most room for improvement was a key focus. This way, I would be able to determine the factors that were most helpful and most costly to SyriaTel.
For each model, we also observed a 2x2 confusion matrix as well as four metrics (accuracy, recall, precision, and F1). The confusion matrices are an easy way to visualize the accuracy of each model. Numbers in the top-left and bottom-right corners represent correct predictions, while the other corners represent incorrect predictions. Accuracy is all about the percentage of predictions (whether or not a customer churned) that were correct. That is a very important metric, but F1 was also a key emphasis, as it considers both precision and recall. Therefore, a high F1 score generally indicates a model that is reliable all-around.

## Models
The first model, which was used only as a preliminary step before diving into models with a higher chance of being a good fit, was a linear regression.
