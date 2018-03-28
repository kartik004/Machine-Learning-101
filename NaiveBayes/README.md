# Naive Bayes Classifier
Naive Bayes is a kind of classifier which uses the Bayes Theorem. It predicts membership probabilities for each class such as the probability that given record or data point belongs to a particular class.  The class with the highest probability is considered as the most likely class. This is also known as **Maximum A Posteriori (MAP)**.

**The MAP for a hypothesis is:**

MAP(H)

= max( P(H|E) )

=  max( (P(E|H)*P(H))/P(E))

= max(P(E|H)*P(H))

P(E) is evidence probability, and it is used to normalize the result. It remains same so, removing it won’t affect.

Naive Bayes classifier assumes that all the features are unrelated to each other. Presence or absence of a feature does not influence the presence or absence of any other feature. We can use Wikipedia example for explaining the logic i.e.,

A fruit may be considered to be an apple if it is red, round, and about 4″ in diameter.  Even if these features depend on each other or upon the existence of the other features, a naive Bayes classifier considers all of these properties to independently contribute to the probability that this fruit is an apple.

In real datasets, we test a hypothesis given multiple evidence(feature). So, calculations become complicated. To simplify the work, the feature independence approach is used to ‘uncouple’ multiple evidence and treat each as an independent one.

##### P(H|Multiple Evidences) =  P(E1| H)* P(E2|H) ……*P(En|H) * P(H) / P(Multiple Evidences)
