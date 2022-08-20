# Credit Risk Analysis (Supervised Machine Learning)
## Overview

The purpose of this project is to use supervised machine learning to determine credit card (default) risk. Credit risk is a generally unbalanced classification problem because good credit loans can easily outnumber riskier loans. In order to select a model of best-fit, six different machine learning models will be run. 

Review of the Accuracy Score to indicate the percentage of correctness.

Examination of the Precision Score to determine the model's performance related to the quality of a positive prediction made by the model.  A perfect precision score of 1.0 means that every result retrieved was relevant. Precision can also be seen as the probability that a randomly selected item which is labeled as "relevant" is a true positive. 

Examination of the Recall Score will indicate how many times the model was able to detect a specific category. A perfect recall score of 1.0 indicates that all relevant documents were retrieved by the search.   


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

### Oversampling: Naive Random

- The Balanced Accuracy Score is 0.64.
- The Precision Score for high credit risk is 0.01.
- The Recall Score for high credit risk is 0.71.

![image](https://user-images.githubusercontent.com/102322707/185753641-16295405-148f-48ea-a6f1-ad50f1de9f82.png)

![image](https://user-images.githubusercontent.com/102322707/185753425-65172a0c-a266-4433-a3ad-fd893d1a69ca.png)

### Oversampling: SMOTE

- The Balanced Accuracy Score is 0.66.
- The Precision Score for high credit risk is 0.01.
- The Recall Score for high credit risk is 0.63.

![image](https://user-images.githubusercontent.com/102322707/185753708-d25217e5-77b0-4fd3-92f8-e22cd718edeb.png)

![image](https://user-images.githubusercontent.com/102322707/185753456-ab0d2492-639c-4b79-a353-7200f17f1ab9.png)

### Undersampling: Cluster Centroids Algorithm

- The Balanced Accuracy Score is 0.66.
- The Precision Score for high credit risk is 0.01.
- The Recall Score for high credit risk is 0.69.

![image](https://user-images.githubusercontent.com/102322707/185753746-b56f5582-13f4-4283-a018-c22d230500c2.png)

![image](https://user-images.githubusercontent.com/102322707/185753531-a7668739-231d-4dd3-a93e-18334fcb85f1.png)

### Combination (Over & Under) Sampling: SMOTEENN

- The Balanced Accuracy Score is 0.54.
- The Precision Score for high credit risk is 0.01.
- The Recall Score for high credit risk is 0.72.

![image](https://user-images.githubusercontent.com/102322707/185753772-f8a51ec1-8836-4e5c-b004-5073d5527d01.png)

![image](https://user-images.githubusercontent.com/102322707/185753575-ff7aaaa9-65fa-4777-a463-2c3995e87496.png)

### Ensemble Learners: Balanced Random Forest Classifier

- The Balanced Accuracy Score is 0.78.
- The Precision Score for high credit risk is 0.03.
- The Recall Score for high credit risk is 0.70.

![image](https://user-images.githubusercontent.com/102322707/185753929-578b0070-fc99-40ab-9ec1-fc64b6442abb.png)

![image](https://user-images.githubusercontent.com/102322707/185753962-28580559-a002-4bd3-8c87-adb4569e8971.png)

![image](https://user-images.githubusercontent.com/102322707/185754081-4dd54a8c-50d6-4e99-a692-288c5b2841ef.png)


### Ensemble Learners:  Easy Ensemble AdaBoost Classifier

- The Balanced Accuracy Score is 0.93.
- The Precision Score for high credit risk is 0.09.
- The Recall Score for high credit risk is 0.92.

![image](https://user-images.githubusercontent.com/102322707/185754018-990fe680-1e69-47dd-b934-c659071d546f.png)

![image](https://user-images.githubusercontent.com/102322707/185754028-1e87c689-e791-49e8-a545-fe31e820bb28.png)


## Summary

In order to determine how well a model is performing, it is best to determine a baseline score to compare the model against. I will surmise that a  baseline score of 80% accuracy (selected in conjuction with the 80/20 rule) would be sufficient, especially since financial default is a costly matter. 

Because there is generally a trade-off in relation to a model's precision or recall, one must consider which is the most important in determining credit risk. Recall tends to be more important where "false negatives" are more costly than "false alarms."  Precision is more important where "false positives" are more costly than "false negatives."  

![image](https://user-images.githubusercontent.com/102322707/185755958-4c89d25c-9a52-4e1d-85ac-9781615bd1bb.png)

In the case of determining credit risk, I would imagine that false negatives, whereby a credit risk is not identified, would be the most costly scenario and therefore the most important (recall is most important).  A low recall score would be indicative of a large number of false negatives! 

I think it would be important to examine the F1 Score, as well, because this score is a weighted average of the true positive rate (recall) and precision score such that the best score is 1.0 and the worst score is 0.0.  The Easy Ensemble AdaBoost Classifier Model had the highest F1 Score of 0.16.


Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.


## Resources
https://www.mage.ai/blog/definitive-guide-to-accuracy-precision-recall-for-product-developers

https://levity.ai/blog/precision-vs-recall

https://www.tandfonline.com/doi/pdf/10.1080/16168658.2021.1925021

https://ntnuopen.ntnu.no/ntnu-xmlui/bitstream/handle/11250/2456356/17904_FULLTEXT.pdf?sequence=1

https://kiwidamien.github.io/interview-practice-with-precision-and-recall.html




