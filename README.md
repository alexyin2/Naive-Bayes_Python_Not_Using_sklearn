# Naive-Bayes
1. This is a practice of helping me to learn the background mathematics in Naive-Bayes.
2. The coding part is based on [lazy programmer](https://github.com/lazyprogrammer)
***

## Introduction of background theory
1. Naive Bayes uses __*Bayesian Theory*__ and assumes that __*each feature is conditionally independent of every other feature*__.
2. We will show the formula below, using the example of detecting whether we should spam an e-mail when it contains specific words.
![image](https://github.com/alexyin2/Naive-Bayes_Python_Not_Using_sklearn/blob/master/Image/NaiveBayesTheory.png)
3. The example showned above doestn't mean that we can only use discreate variables. 
4. We can also use continuous variables, just remember that the prior probability is turned into a probability distribution, same as what we've learned in Bayesian Theory.
***
## Dealing with 0 probabilites
1. If you've done some practice on real data, you may notice that there's a problem in Naive Bayes.
2. When one of the probabilites is 0, the whole posterior will become 0.
3. One way to deal with this kind of situation is to use the add-one smoothing, also known as Laplace smoothing.
4. We will show how this solution works below:
![image](https://github.com/alexyin2/Naive-Bayes_Python_Not_Using_sklearn/blob/master/Image/One-addSmoothing.png)
