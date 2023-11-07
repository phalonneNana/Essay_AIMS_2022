# Goal
The challenge of detecting credit card fraud is connected to various aspects that may prohibit the direct
deployment of certain prediction approaches, and hence, deserves special consideration. The challenging
factor in our situation is the class imbalance. It can
prohibit learning algorithms from learning normally, as the system fails to detect or simply ignores the
minority class. To address this issue, we present a novel
regularization strategy that uses two factors which are mean divergence and
variance divergence of the model’s output distribution (considering a student -
t distribution). The proposed terms are added to the loss function, and they are considered
as penalties terms to the model against the majority and for the minority class.


# Dataset
The dataset used in this research represents credit card transactions done by European cardholders in
September 2013. It contains the transactions from the last two days by several users, with 492 frauds
out of 284,807 total transactions. It contains only numerical input variables which are the result of a
PCA transformation. Unfortunately, due to confidentiality issues, we have not been provided with the
original features, and more background information about the data.As this piece of works entails, the
difficult aspect is that it is significantly unbalanced, with the positive class (frauds) accounting only
for 0.172 percent of all transactions. you can find it here: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud


# Results
Our methods have been compared here with the random Oversampling. n view of our results, it appears that both methods give acceptable accuracy and F1-results and allow
the algorithm to make good predictions and also it emerges that the more the degrees of freedom
increase the more the predictions are bad because the majority of the good predictions is obtained for
the smallest degree of freedom; In this logic, we can thus say that the student - t distribution applied to
our data is reliable for small degrees of freedom.  Nevertheless, the oversampling method has slightly
better results due to the amount of sample.
### Finally, we can say that our error function containing the regularization terms is acceptable with respect to the the different tests.


# Good Reading😁
