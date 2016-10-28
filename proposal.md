# Lazy Boosting

AdaBoost has remarkalble guranteees for learning given that it base
classifiers are weak learners. Traditionally boosting stumps have been used due
to their efficiency and simplicity. The drawback of using boosting stumps is
that they are not weak classfiers as they cannot give > 1/2 accuracy on all
distributions of training data. One could use more coomplex base classifiers,
but that could result in overfitting and increased asymptotic complexity.

To overcome this situtation we propose using complex base classifiers which are
weak learners. But, instead of returning the optimal classifier at each
AdaBoost step, we will return a classifier which is just good enough (> 1/2)
accuracy. We hope that this will prevent over-fitting and not having to find
the optimal classifier will allow us to have a lower asymtpotic complexity.
We initially plan to study simple families of functions as weak base classifiers
such as hyperplanes and hyperplanes passing through origin. We hope to show
that all the results presented for AdaBoost will still hold. In addition
to that we will investigate efficient randomized or deterministic algorithms 
to find base classifiers which are just good enough. 
