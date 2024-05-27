# Distributed computing

Przemysław Szufel

Note that this is a virtual environment from distributed computing.
For GPU there is a separate environment.

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
- Jupyter notebook: [Julia_Parallel_Distributed_2024_EC.ipynb](Julia_Parallel_Distributed_2024_EC.ipynb)
- Slides: [Julia_Parallel_Distributed_2024_EC.pptx](Julia_Parallel_Distributed_2024_EC.pptx)