# MickowskiEngine-Installtion_Ubuntu20-04_Cuda_11-6
Installtion of MickowskiEngine on Ubuntu 20.04 and Cuda 11.6
Requirement

1. Ubuntu 20.04
2. Cuda 11.6(Toolkit)


Open Terminal 
```bash
conda create -n py3-mink python=3.9
conda activate py-mink
conda install openblas-devel -c anaconda
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
conda install -c conda-forge setuptools=59.8.0
conda install -c conda-forge numpy=1.22.0
conda list setuptools
conda list numpy
conda install -c conda-forge ninja
export CUDA_HOME=/usr/local/cuda-11.6
export BLAS_INCLUDE_DIRS=${CONDA_PREFIX}/include
export BLAS=openblas
pip install -U git+https://github.com/NVIDIA/MinkowskiEngine -v --no-deps
```
    
