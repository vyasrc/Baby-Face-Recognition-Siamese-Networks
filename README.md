# Baby-Face-Recognition-Siamese-Networks
  A New-Born Baby Face Recognition Using Siamese Neural Networks and One Shot Learning.                                                       
### Introduction :-                
Biometric recognition of new-born babies is an opportunity for the realization of several useful applications, such as improved security against swapping and abduction, accurate census, and effective drug delivery. Here we implement a method for learning Siamese neural networks which employ a unique structure to naturally rank similarity between inputs. Once a network has been tuned, we can then capitalize on powerful discriminative features to generalize the predictive power of the network not just to new data, but to entirely new classes from unknown distributions. One particularly interesting task is classification under the restriction that we may only observe a single example of each possible class before making a prediction about a test instance. This is called one-shot learning and it is the primary focus of our model presented in this work.

### Convolutional Architecture :-
![](https://github.com/vyasrc/Baby-Face-Recognition-Siamese-Networks/blob/master/CA%20(2).png)

### Overall Architecture :-
![](https://github.com/vyasrc/Baby-Face-Recognition-Siamese-Networks/blob/master/combined%20(2).png)

### 10-way One-Shot Classification :-
To train our verification network, we put together data set size with 16 random training examples
by sampling random same and different pairs for each iteration. We set aside sixty
percent of the total data for training.We fixed a uniform number of training examples per
baby so that each baby receives equal representation during optimization, although this is
not guaranteed to the individual baby faces within each baby class. By adding affine distortions,
we also produced an additional copy of the data set corresponding to the augmented
version of each of these sizes. We added eight transforms for each training example, so the
corresponding data sets have 128 effective examples per iteration. To monitor performance
during training, we create a random validation set for verification with 600 example pairs
taken from 33 baby classes each class with 10 baby face images. By this strategy we were
able to generate a set of 60 10-way one-shot recognition trials for the validation set which
mimic the target task on the testing set. In practice, this second method of determining when
to stop was at least as effective as the validation error for the verification task so we used it as
our termination criterion. We reserved the last 30 babies with 4 baby faces as testing set.In the graph below, we list the validation accuracy during training.

![](https://github.com/vyasrc/Baby-Face-Recognition-Siamese-Networks/blob/master/combined%20(3).png)

### Results :-
![](https://github.com/vyasrc/Baby-Face-Recognition-Siamese-Networks/blob/master/combined%20(4).png)
* Test Accuracy - 78.34%
* Validation Accuracy - 76.67%


### Conclusion :-
We have presented a strategy for performing one-shot classification by first learning deep convolutional Siamese neural networks for verification. We considered training for the verification task by processing image pairs and their distortions using a global affine transform.
