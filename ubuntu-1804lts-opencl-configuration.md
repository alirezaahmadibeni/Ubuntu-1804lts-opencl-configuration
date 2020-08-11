**Configure Ubuntu 18.04LTS as an OpenCL development platform:**

With OpenCL, the [installable client drivers](https://www.khronos.org/news/permalink/opencl-installable-client-driver-icd-loader) (ICDs) are normally issued with the accelerator's device drivers, namely:

1. AMD's.
2. Intel's.


**Practical example: Pythonic access to the OpenCL parallel computation API:**

Fetch the source:

    git clone https://github.com/inducer/pyopencl.git

Install build dependencies:

    sudo apt-get install opencl-headers
    sudo apt-get install ocl-icd-opencl-dev
    sudo apt-get install clinfo
    sudo pip3 install pyopencl

Erros:

    CLINFO Number of Platforms 0 Error
    Running CLINFO Returns The Error “Number of Platforms – 0” Even With AMD Drivers Installed
    This happens in Ubuntu Server 18.04 and most likely other versions.  To fix it run the following:

    sudo apt install mesa-opencl-icd

**Test:**











