# pythonml-cuda11x-win64
My custom environment for running local GPU-accelerated TensorFlow, PyTorch, Keras, and Scikit-learn applications on Windows computer. Based on yml file by A. Geron for [Hands on ML 3](https://github.com/ageron/handson-ml3)

I originally ran into issues installing GPU-capable versions of packages to learn TensorFlow and Pytorch due to compatibility issues. I thought I'd share the environment I use on my local machine with 3080 GPU, Win 10, CUDA 11x. The .yml file is based on https://github.com/ageron/handson-ml3/blob/main/environment.yml and has been modified to allow GPU-enabled execution of deep learning models using either TensorFlow or PyTorch. 

GPU Drivers were installed from  [GPU driver](https://www.nvidia.com/Download/index.aspx)

I chose Game Ready Driver v 536.40, NVIDA GPU Computing Toolkit v11.2, and Visual Studio 2019 for compatability with my other mexcuda projects in MATLAB 2022b.

### Clone this repository or download the the .yml file to build the environment.

    $ git clone https://github.com/SilentAndromeda/pythonml-cuda11x-win64.git
    $ cd pythonml-cuda11x-win64

### Run the following commands in a conda terminal.

    $ conda env create -f environmentGPU.yml
    $ conda activate ml-gpu
    $ python -m ipykernel install --user --name=python3

### You should now be able to start developing GPU-accelerated models in Juyter lab! 

    $ jupyter lab
