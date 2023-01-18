# -Certified-bagging-model-data-poisoning-attack

The goal of project is to find the maximal poisoning size r such that the network still predicts label l for x when trained on the poisoned training dataset with at most r poisoned training examples.

We poisoned the training network by changing the label. First, we created poisoning_label function to change the label to 0. If the label was equal to 0, we changed it to 1 instead. This function required two inputs which are label array and poisoning size. Secondly, we created count_label function to check each digit label before and after we poisoned the training label. Finally, we created bagging_accuracy function to calculate the model accuracy at the end.

Conclusion

  In this project, we studied the paper which introduced the bound of data poisoning attack that the CNN network with bagging ensemble method still can predict the same label for testing examples. In this work, we have tested with the code that they provided from the paper. Even though our results are not the same as their paper, we observed the same trend on poisoning size that shows the zero certified accuracy and the k value. When k is large, the certified accuracy is high and then falls significantly when the poisoning size rises. Moreover, we conducted the label poisoning attack with slight adjustments to the CNN network by changing the model’s optimizer. The results show a different trend from the paper’s result. We observed our accuracy markedly drops and then suddenly increases after the same poisoning size which we need to further investigate in the future.
