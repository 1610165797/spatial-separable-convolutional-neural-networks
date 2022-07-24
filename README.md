# MobileNets

Implementation of the MobileNets CNN model in CUDA
The main branch is the original design.
For accelerated design, please see branch kernel_layout.

Our Report Paper: https://github.com/shuanggewang/spatial-separable-convolutional-neural-networks/blob/kernel_layout/Spatial_Separable_Convolutional_Neural_Networks_Parallelization_and_Accelerations.pdf

MobileNets Paper: https://arxiv.org/abs/1704.04861


## Installation Procedures
1. Copy the entire repository to your workspace (CARC). 
2. No extra libraries or dependencies are required.
3. Run the following commands in exact order.
```
module load nvidia-hpc-sdk
nvcc MobileNets_host.cu -o MobileNets_host
sbatch job.sl
cat gpujob.out
```

