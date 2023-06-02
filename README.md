# A Benchmarking Platform for Atomic Learned Indexes

This repository provides a benchmarking platform to evaluate how Feed Forward Neural Networks can be effectively used as index data structures. That is, how well in terms of time and space, those Networks can solve the well known predecessor problem, i.e., searching for an element in a sorted table. In theory, those networks, with RELU activators,  are able to approximate any function [1] , including the one needed to solve predecessor search. Then, a simple binary search concludes the task.  
  
The scenario we have considered is in memory data and batch queries, which is a fundamental one, as outlined in [ CSS].  
  
We include:  
  
* 3 [Neural Networks](https://github.com/DomenicoAmato01/A-Benchmarking-Platform-for-Atomic-Learned-Indexes/tree/master/src/Neural_Nets) with different number of layers  

The datsets used for benchmarking can be downloaded [here](https://osf.io/ernyh/?view_only=ef751aaced30438397d90dee2a154747).
  
## Directory Structure
    .
    └── src                    # Source Directory
        └── Neural_Nets           # Neural Nets Scripts Directory
              └── mdls                # Models Directory   
                   └──json               # Neural Nets Json
        
    
 ## Implementations
 
 All implementation and execution details are provided inside the source directory.  
 The code provided here presents different execution scenarios, including GPU Cuda Cores and Tensor Core
 
 
 ## Cite

If you use this benchmark in your own work, please cite us:

```

@InProceedings{10.1007/978-3-031-08223-8_10,
 author="Amato, Domenico and Lo Bosco, Giosu{\'e} and Giancarlo, Raffaele",
 title="On the Suitability of Neural Networks as Building Blocks for the Design of Efficient Learned Indexes",
 booktitle="Engineering Applications of Neural Networks",
 year="2022",
 publisher="Springer International Publishing",
 address="Cham",
 pages="115--127",
 isbn="978-3-031-08223-8"
}

@misc{amato2022standard,
      title={On the Suitability of Neural Networks as Building Blocks for the Design of Efficient Learned Indexes}, 
      author={Domenico Amato and Giosuè Lo Bosco and Raffaele Giancarlo},
      year={2022},
      eprint={2203.14777},
      archivePrefix={arXiv},
      primaryClass={cs.DS}
}
 
## Bibliography
[1] Hanin, B. and Sellke, M. (2017). Approximating continuous functions by ReLU nets of minimal
width. arXiv preprint arXiv:1710.11278.

