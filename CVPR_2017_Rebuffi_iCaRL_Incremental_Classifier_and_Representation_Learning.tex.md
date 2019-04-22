# iCarRL: Incremental Classifier and Representation Learning.

__Sylvestre-Alvise Rebuffi- University of Oxford/IST Austria__

This paper proposed a method that learn data representation and Incremenatal Learning Classifier (using 32-Layer ResNet)
simutaneously. 

**Data Representation**. For every incremental step, the samples (images) of each class for old and new classes are constructed. The total samples must not be excceed K, thus each class will have max $m =K/t$, given t classes are presented.
