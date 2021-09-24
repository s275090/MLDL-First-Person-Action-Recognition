# MLDL-First-Person-Action-Recognition
This is a project carried out in the Machine Learning and Deep Learning course held by Barbara Caputo

#### OVERVIEW
The goal of the project is to become familiar with the task of action recognition. The student should understand the general approach to tackle the video recognition task and the problems that they may have dealing with the first-person data.  Before starting, the student should read [1] in order to get familiar with the following terms: Optical Flow, Recurrent Neural Network (RNN) and Class Activation Maps (CAM). The student should be able to replicate some experiments proposed in [1]. As the next step, the student should implement the self-supervised task as described in [2]. For the last part of the project, the student should propose a variation for the project, taking inspiration from a set of possible ideas.

#### OUR IMPLEMENTATION
For our implementation, we propose to use sequence sorting as self-supervised task for training a CNN. 

Our hypothesis is that appearance variations and temporal coherence in videos offer rich supervisory signals for representation learning. Predict variations pixels is challenging. To avoid this complex task of predicting high-dimensional video frames, we use sequential verification. So, we formulate the sequence sorting problem as a multi-class classification task. 
Then to further reduce the complexity, we reduce number of frames to be reorder and the number of possible permutations by following the maximum Hamming distance . 
