
# iCarRL: Incremental Classifier and Representation Learning.

__Sylvestre-Alvise Rebuffi- University of Oxford/IST Austria__

__CVPR_2017__

This paper proposed a method that learns data representation and Incremental Learning Classifier (using 32-Layer ResNet) simutaneously. The paper experiments on image datasets (CIFAR100, ILSVRC).
. 
<img src="Figure_1.jpg" width="400">

**Training/Testing Procudure**. The image dataset is split into training/testing sets with a ratio (let's say 90/10). The training is conducted online, where a portion of training sets is fed into the network in each training step. For example, at  1st training step, we can feed 2 classes of dog an cat (600 images/class); at 2nd training step, images of next 2 classes are fed into the network. We can also change the number of classes in each training step to 5,10,...etc. The trained networks in each training steps are tested on testing datasets (10% of data). However, we only test on images of the trained classes. 

**Data Representation**. For every incremental step, the samples (images) of each class for old and new classes are constructed. The total samples must not be excceed K, thus each class will have max $m =K/t$, given t classes are presented.
<img src="Figure_2.jpg" width="400">

**Incremental Learning** 
Given m samples of each class (old and new ones), the steps of incremental learning is as follows:
1. All samples are gathered into set $D$
2. Calculate network outputs with pre-update network parameters. These outputs are used to minimize
the distillation loss in next steps.
3. All samples in set $D$ are used to minimize the loss function consisting of **distillation loss** and **classification loss**. The intuition of distillation loss is that we want the new (updated) network weights to generate the same outputs for samples of old classes in step 2. This helps solve the catastrophic forgeting problem. At the same time, the classification loss discriminates samples in entire classes. 
The algorithm is as followed. 
<img src="Figure_3.jpg" width="400">

**Classification**: The idea is simmilar to the concept of K-Means. The mean of exemplars (samples that are selected) are calculated using the feature vector of each exemplar. The predicted class of a testing image is the nearest class to that image in feature spaces. The algorithm is below:
<img src="Figure_4.jpg" width="400">
The arguments for using nearest-mean-of-exemplars instead of usual network outputs (softmax) are not clear in this paper. However, the ablation study shows the improved accuracy of using nearest-mean-of-exemplars.


**Results.** 
1. Compare with previous methods on CIFAR100 and ILSVRC datasets. 
<img src="Figure_5.jpg" width="800">

2. **Confusion matrices**

3. **Ablation study:**
 hybrid1- use classification outputs.
 hybrid2- not use distillation loss.
 hybrid3- not use distillation loss + exemplars for classication, but use exemplars for represetnation learning.
 lwF.MC- a related method.
<img src="Figure_6.jpg" width="400">




```python

```
