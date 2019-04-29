# Transfer_Continuous_Unsupervised_Learning

# Domain Adaption
1. **DAMS** :Domain Adaptation with Multiple Sources.[[NIPS2009](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/35079.pdf)].
1. NIPS_2014_Hinton_Distilling the knowledge in a neural network. [[paper](https://arxiv.org/abs/1503.02531?context=cs)],[code],[[video](https://www.youtube.com/watch?v=skHpJ-oTi6o)].
1. ArXiv_2016_Rusu_Deepmind_Progressive Neural Networks. [[paper](https://arxiv.org/pdf/1606.04671.pdf)], [[code](https://github.com/mhsamavatian/ProgressiveNeuralNet)]
1. ArXiv_2016_Beyond Sharing Weights for Deep Domain Adaptation. [[paper](https://arxiv.org/pdf/1603.06432.pdf)],[[PAMI_2019](https://infoscience.epfl.ch/record/253629/files/main.pdf;)],[[code]], [[summary]].
1. ECCV_2016_PAMI_2018_Li_Learning without Forgetting.[[paper](https://arxiv.org/pdf/1606.09282.pdf)],[code](https://github.com/lizhitwo/LearningWithoutForgetting),**[[summary](https://github.com/trungmanhhuynh/Transfer_Continuous_Unsupervised_Learning/blob/master/ECCV_2016_Li_Learning_Without_Forgetting/ECCV_2016_Li_LwF.ipynb)]**
1. CVPR_2016_Xiao_Learning Deep Feature Representations with Domain Guided Dropout for Person Re-identification.[[paper](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Xiao_Learning_Deep_Feature_CVPR_2016_paper.pdf)],[[code](https://github.com/Cysu/dgd_person_reid)],**[[summary](https://github.com/trungmanhhuynh/Transfer_Continuous_Unsupervised_Learning/blob/master/CVPR_2016_Xiao_Domain_Guided_Dropout/CVPR_2016_Xiao_Domain_Guided_Dropout.ipynb)]**
1. CVPR_2017_Rebuffi_iCaRL: Incremental Classifier and Representation Learning. [[paper](http://openaccess.thecvf.com/content_cvpr_2017/papers/Rebuffi_iCaRL_Incremental_Classifier_CVPR_2017_paper.pdf)],[[code](https://github.com/srebuffi/iCaRL)],**[[summary](https://github.com/trungmanhhuynh/Transfer_Continuous_Unsupervised_Learning/blob/master/CVPR_2017_Rebuff/CVPR_2017_Rebuff.ipynb)]**
1. ECCV_2018_Castro_End-to-End Incremental Learning [[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Francisco_M._Castro_End-to-End_Incremental_Learning_ECCV_2018_paper.pdf)], [[code]()].
1. Neurorobotics_2018_Parisi_Lifelong Learning of Spatiotemporal Representations with Dual-Memory Recurrent Self-Organization. [[paper](https://arxiv.org/pdf/1805.10966.pdf)],[[code](https://github.com/giparisi/GDM)].
1. Neurocomputing_2018_Mei_Wang_Deep_Visual_Domain_Adaptation_A_Survey,[[paper](https://arxiv.org/pdf/1802.03601.pdf)],[code].
1. Arvix_2019_Aljundi_Online continual learning with no task boundaries.[[paper](https://arxiv.org/pdf/1903.08671.pdf)],[code].
1. NN_2019_Parisi_Continual lifelong learning with neural networks: A review. [[paper](https://arxiv.org/abs/1802.07569)],[code].

# Key words: 
**Transfer Learning**. The idea is that instead of training the network from scratch, one can take a pre-trained networks and adapt it 
to solve their own tasks. There are two variations:
 - Same domain, different tasks. For example, using the same image datasets (e.g. ImageNet), but a trained network on object detection
 can be used for scene classification or depth estimation.
 - Same tasks, different domains. This is called **Domain Adaption**. Object recognition for different datasets, or human tracking/trajectory prediction from static vs dynamic video scenes. 
 - Different domain, different tasks?.

**Domain Adaption**

**Continual Learning**

**Multi-tasks Learning**

**Lectures**
1. [Foundations of Unsupervised Deep Learning (Ruslan Salakhutdinov, CMU)](https://www.youtube.com/watch?v=rK6bchqeaN8)

**Other resources:**
1. https://vlomonaco.github.io/core50/strategies.html#ref
1. https://github.com/barebell/DA

# Summary 
**Continous/Continual/Incremental Learning**

A truly incremental deep learning approach for classification (Castro2018 et al) is characterized by its:
 - ability to being trained from a flow of data, with classes appearing in any order, and at any time 
 - good performance on classifying old and new classes.
 - reasonable number of parameters and memory requirements for the model.
