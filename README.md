# Transfer_Continuous_Unsupervised_Learning

1. NIPS_2014_Hinton_Distilling the knowledge in a neural network. [[paper](https://arxiv.org/abs/1503.02531?context=cs)],[code],[[video](https://www.youtube.com/watch?v=skHpJ-oTi6o)].
1. CVPR_2017_Rebuffi_iCaRL: Incremental Classifier and Representation Learning. [[paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Rebuffi_iCaRL_Incremental_Classifier_CVPR_2017_paper.pdf)],[[code](https://github.com/srebuffi/iCaRL)], [[summary](https://github.com/trungmanhhuynh/Transfer_Continuous_Unsupervised_Learning/blob/master/CVPR_2017_Rebuff/CVPR_2017_Rebuff.pdf)]
1. ECCV_2018_Castro_End-to-End Incremental Learning [[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Francisco_M._Castro_End-to-End_Incremental_Learning_ECCV_2018_paper.pdf)], [[code]()].
1. Neurorobotics_2018_Parisi_Lifelong Learning of Spatiotemporal Representations with Dual-Memory Recurrent Self-Organization. [[paper](https://arxiv.org/pdf/1805.10966.pdf)],[[code](https://github.com/giparisi/GDM)].
1. Arvix_2019_Aljundi_Online continual learning with no task boundaries.[[paper](https://arxiv.org/pdf/1903.08671.pdf)],[code].
1. NN_2019_Parisi_Continual lifelong learning with neural networks: A review. [[paper](https://arxiv.org/abs/1802.07569)],[code].

**Lectures**
1. [Foundations of Unsupervised Deep Learning (Ruslan Salakhutdinov, CMU)](https://www.youtube.com/watch?v=rK6bchqeaN8)

**Other resources:**
1. https://vlomonaco.github.io/core50/strategies.html#ref

# Summary 
**Continous/Continual/Incremental Learning**

A truly incremental deep learning approach for classification (Castro2018 et al) is characterized by its:
 - ability to being trained from a flow of data, with classes appearing in any order, and at any time 
 - good performance on classifying old and new classes.
 - reasonable number of parameters and memory requirements for the model.
