# iCarRL: Incremental Classifier and Representation Learning.

__Sylvestre-Alvise Rebuffi- University of Oxford/IST Austria__

This paper proposed a method that learn data representation and Incremenatal Learning Classifier (using 32-Layer ResNet)
simutaneously. 

**Data Representation**. For every incremental step, the samples (images) of each class for old and new classes are constructed. The total samples must not be excceed K, thus each class will have max <img src="/tex/d2f9cd76f82f6e0b3482924f710b3fec.svg?invert_in_darkmode&sanitize=true" align=middle width=64.72979369999999pt height=24.65753399999998pt/>, given t classes are presented.
