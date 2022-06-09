# High Performance Computing for Machine Learning

#### led by Dr. Chuck Pavloski and Dr. Justin Petucci from the [ICDS RISE Team](https://www.icds.psu.edu/computing-services/rise/rise-team-members/) 
#### Astroinformatics Summer School 2022 
#### Organized by [Penn State Center for Astrostatistics](https://sites.psu.edu/astrostatistics/)

-----
This repository contains the following computational notebooks and supporting files: 
- gpu_linear_algebra.ipynb ([Jupyter notebook](https://github.com/Astroinformatics/HighPerformanceComputing/blob/main/gpu_linear_algebra.ipynb)):  Compare performance of CPU and GPU for common linear algebra tasks
- gpu_neuralnetwork.jl ([Pluto notebook](https://astroinformatics.github.io/HighPerformanceComputing/gpu_neuralnetwork.jl.html)):  Compare performance of CPU & GPU for training a neural network

Files ending in .jl are Pluto notebooks and files ending in .ipynb are Jupyter notebooks, both written in Julia.
Labs do not assume familiarity with Julia.  While it can be useful to "read" selected portions of the code, the lab tutorials aim to emphasize understanding how algorithms work, while minimizing need to pay attention to a language's syntax.

---
## Running Labs
Instructions will be provided for students to run labs on AWS severs during the summer school.  Below are instruction for running them outside of the summer school.  Note that these labs require running on a system with an CUDA-compatiable GPU.

### Running Pluto notebooks on your local computer
Summer School participants will be provided instructions for accessing a Pluto server.  Others may install Julia and Pluto on their local computer with the following steps:
1.  Download and install current version of Julia from [julialang.org](https://julialang.org/downloads/).
2.  Run julia
3.  From the Julia REPL (command line), type
```julia
julia> using Pkg
julia> Pkg.add("Pluto")
```
(Steps 1 & 3 only need to be done once per computer.)

4.  Start Pluto
```julia
julia> using Pluto
julia> Pluto.run()
```
5.  Open the Pluto notebook for your lab

### Running Jupter notebooks with a Julia kernel on your local computer
Summer School participants will be provided instructions for accessing JupyterLab server.  
Others may install Python 3 and Jupyter (or JupyterLab) on their local computer or use [Google Colab](https://colab.research.google.com/) to open the Jupyter notebooks.  Probably the easiest way to do that is with the following steps:
1.  Download and install current version of Julia from [julialang.org](https://julialang.org/downloads/).
2.  Run julia
3.  From the Julia REPL (command line), type
```julia
julia> using Pkg
julia> Pkg.add("IJulia")
```
(Steps 1 & 3 only need to be done once per computer.)

4.  Start Jupyter
```julia
julia> using IJulia
julia> notebook()
```
5.  Open the Jupyter notebook for your lab

---
## Additional Links
- [GitHub respository](https://github.com/Astroinformatics/SummerSchool2022) for all of Astroinformatics Summer school
- Astroinformatics Summer school [Website & registration](https://sites.psu.edu/astrostatistics/astroinfo-su22/)

## Contributing
We welcome people filing issues and/or pull requests to improve these labs for future summer schools.
