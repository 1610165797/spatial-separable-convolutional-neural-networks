# MobileNets

Implementation of the MobileNets CNN model in CUDA
The main branch is the original design.
For improved design, please see branch kernel_layout.

MobileNets Paper: https://arxiv.org/abs/1704.04861

Our Report Paper: https://github.com/1610165797/spatial-separable-convolutional-neural-networks/blob/main/Spatial%20Separable%20Convolutional%20Neural%20Networks%20Parallelization%20and%20Acceleration.pdf

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

