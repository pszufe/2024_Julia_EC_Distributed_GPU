# Selected feature of GPU computing in Julia

Przemysław Szufel

This is a separate virtual environment from GPU computing.
Those codes and libraries can only be installed and run on a machine with an nvidia CUDA GPU.

In order to install the dependecies for this subproject run the Julia console or in the command line (run command **julia** in the project folder). Once Julia interpreter is running paste the following Julia code:
```
using Pkg
pkg"activate ."
pkg"instantiate"   # installs all packages and dependecies.
```

For this code typically the Jupyter notebook will be started in multithreaded mode:
```
using IJulia
ENV["JULIA_NUM_THREADS"]=4
notebook(dir=".")
```

Materials:
- Quick demo to get the first feeling: [cudaarraysdemo.ipynb](cudaarraysdemo.ipynb)
- Overview of CUDA functionality (based on https://cuda.juliagpu.org/): [CudaOverview.ipynb](CudaOverview.ipynb)