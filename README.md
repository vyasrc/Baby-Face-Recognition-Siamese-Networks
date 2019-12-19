# Baby_Face_Recognition_Siamese-Networks
  A New-Born Baby Face Recognition Using Siamese Neural Networks and One Shot Learning.                                                       
### Introduction :-                
Biometric recognition of new-born babies is an opportunity for the realization of several useful applications, such as improved security against swapping and abduction, accurate census, and effective drug delivery. Here we implement a method for learning Siamese neural networks which employ a unique structure to naturally rank similarity between inputs. Once a network has been tuned, we can then capitalize on powerful discriminative features to generalize the predictive power of the network not just to new data, but to entirely new classes from unknown distributions. One particularly interesting task is classification under the restriction that we may only observe a single example of each possible class before making a prediction about a test instance. This is called one-shot learning and it is the primary focus of our model presented in this work.

### Convolutional Architecture :-
![](https://github.com/vyasrc/Baby-Face-Recognition-Siamese-Networks/blob/master/CA%20(2).png)

### Overall Architecture :-
![](https://github.com/vyasrc/Baby-Face-Recognition-Siamese-Networks/blob/master/combined%20(2).png)

### 10-way One-Shot Classification :-
![](https://github.com/vyasrc/Baby-Face-Recognition-Siamese-Networks/blob/master/combined%20(3).png)

### Results :-
![](https://github.com/vyasrc/Baby-Face-Recognition-Siamese-Networks/blob/master/combined%20(4).png)
* Training Accuracy - 78.34%
* Validation Accuracy - 76.67%

### Conclusion :-
We have presented a strategy for performing one-shot classification by first learning deep convolutional Siamese neural networks for verification. We considered training for the verification task by processing image pairs and their distortions using a global affine transform.
