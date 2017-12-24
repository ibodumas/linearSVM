# linearSVM
This project involves the implementation of efficient and effective LinearSVC on MNIST data set. The MNIST data comprises of digital images of several digits ranging from 0 to 9. Each image is 28 x 28 pixels. Thus, the data set has 10 levels of classes.

SVC in Sklearn implement the “one-against-one” methodology for multi-class classification. Hence given n classes, n*(n - 1)/2 classifiers would be modeled. Thus, in the case of MNIST dataset, there will be a total of 45 classifiers.

To provide a consistent interface with other classifiers, the decision_function_shape option allows aggregating the results of the “one-against-one” classifiers to a decision function of shape (n_samples, n_classes).

For LinearSVC, performs “one-vs-the-rest” multi-class classification. Hence, a total of n classifier, However, only one classifier will be trained if there are two classes. Thus, in this project 10 classifiers are modeled for LinearSVC.

