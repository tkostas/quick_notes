# System Administration


## Setup NVIDIA, Cuda, cuDNN drivers
* Install CUDA Toolkit, which will also install Nvidia drivers, so that you match the versions, 
  following the instructions in the developers pages https://developer.nvidia.com/cuda-11-8-0-download-archive. 
  Make sure though that cuDNN supports this version, which might mean that you don't use the last one.
* Manually instal cuDNN -> https://askubuntu.com/a/76727. For cuDNN 8.6 I used:
  * `sudo cp include/* /usr/local/cuda/include`  # copy all from the include not just the cudnn.h
  * `sudo cp lib/libcudnn* /usr/local/cuda/lib64`
  * `sudo chmod a+r /usr/local/cuda/lib64/libcudnn*`
  * `cat /usr/local/cuda/include/cudnn_version.h | grep CUDNN_MAJOR -A 2` --> check installed version

Check nvidia driver/cuda versions: `nvidia-smi`. 

Check cuDNN version `cat /usr/local/cuda/include/cudnn_version.h | grep CUDNN_MAJOR -A 2`

See also:
* https://praveenkrishna.medium.com/downgrade-cuda-for-tensorflow-gpu-17831db59099
* https://www.tensorflow.org/install/source#gpu
* https://github.com/mjiUST/driver_cuda_cudnn
