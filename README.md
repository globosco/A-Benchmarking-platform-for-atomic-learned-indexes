# A Benchmarking Platform for Atomic Learned Indexes

This repository provides a benchmarking platform to evaluate how Feed Forward Neural Networks can be effectively used as index data structures. That is, how well in terms of time and space, those Networks can solve the well known predecessor problem, i.e., searching for an element in a sorted table. In theory, those networks, with RELU activators,  are able to approximate any function [1] , including the one needed to solve predecessor search. Then, a simple binary search concludes the task.  
  
The scenario we have considered is in memory data and batch queries, which is a fundamental one, as outlined in [ CSS].  
  
We include:  
  
* 3 [Neural Networks](https://github.com/DomenicoAmato01/A-Benchmarking-Platform-for-Atomic-Learned-Indexes/tree/master/src/Neural_Nets) with different number of layers  

The datsets used for benchmarking are in http://math.unipa.it/lobosco/NNLI/
  
## Directory Structure
    .
    └── src                    # Source Directory
        └── Neural_Nets           # Neural Nets Scripts Directory
              └── mdls                # Models Directory   
                   └──json               # Neural Nets Json
        
    
 ## Implementations
 
 All implementation and execution details are provided inside the source directory.  
 The code provided here presents different execution scenarios, including GPU Cuda Cores and Tensor Core
 
 ## Bibliography
 [1] Hanin, B. and Sellke, M. (2017). Approximating continuous functions by ReLU nets of minimal
width. arXiv preprint arXiv:1710.11278.

