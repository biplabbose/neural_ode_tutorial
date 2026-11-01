### Learning Neural ODE using Julia

Julia is a programming language for scientific and numerical computing. We will use Julia to train a neural ODE and use it. 

A Jupyter-notebook with the Julia code is provided. You can use that for the computation. That notebook also explains the algorithm. 

#### Install Julia

It is very easy to install and run Julia. Please follow the instructions on the official Julia [page for installation](https://julialang.org/downloads/).  I would recommend you to use Linux - a Linux distro like Ubuntu or WLS within Windows.

Here, I provide the essential steps on Linux. The easiest way to install and update Julia on Linux is though `juliaup`. Install it using the following command on the terminal: 

`curl -fsSL https://install.julialang.org | sh`

Upon installation check the status:
`julia --version`
`juliaup status`

To update Julia use:
`juliaup update`

#### Install Jupyter

Follow the instructors  on the [official Jupyter page](https://jupyter.org/install) to install Jupyter lab. On Linux use: 
`pip install jupyterlab`

Your Linux distro may not allow `pip` to install Jupyter lab. You can use `pipx`. Install `pipx` followed by Jupyter lab.
`sudo apt update`
`sudo apt install pipx`

If required, run the following command to ensure that applications installed via `pipx` can be run globally from your terminal:
`pipx ensurepath`

To install Jupyter lab:
`pipx install jupyterlab`

#### Using Julia

One can use Julia through multiple modes - interactively on Julia REPL, running a Julia script (with extension.`.jl`), and through Jupyter notebook. In this tutorial we will use Jupyter notebook. 

Here, we discuss how you can use Julia REPL to install Julia packages. On the terminal execute:
`julia`

This will take you to Julia REPL and the prompt will change to `julia>`. You can now use the REPL interactively. For example, try doing a calculation: `2+3`. It will return `5`. 

To install a package, we need to go into the Package mode. To do so, press `]` at the Julia REPL prompt. The prompt will change to `pkg>` . To check the installed packages, execute the following at the Package prompt:
`status`

To install a package use:
`add <PackageName>`

To run Julia in a Jupyter notebook we need the Julia kernel for Jupyter. For that install the `IJulia` package. At the Package prompt execute:
`add IJulia`

You can install a package at the Julia prompt also:
`using Pkg`
`Pkg.add("IJulia")`

#### Use the Jupyter Notebook

**Important**: Make sure that you have already installed `IJulia`.

Download the Jupyter notebook `neural_ode_tutorial.ipynb` and place it at suitable directory or folder. Go to that folder and start the Linux terminal from that folder. 

Start Jupyter lab by using the following command at the Linux terminal (Not in Julia REPL):
`jupyter-lab` or `jupyter lab`

Jupyter will open on your default web browser. In case it does not open, go back to the Linux terminal. You will find URLs given. Copy and paste one of the URLs on the web browser.

All the files in the folder could be seen and browsed from the left-hand panel of the Jupyter lab. Double click on the notebook (`neural_ode_tutorial.ipynb`). It should open on the right-hand panel of Jupyter lab.

#### How to use Jupyter Notebook

This notebook of cells with contents. There are two type of contents - plain texts (in markdown) explaining the code and  Julia code. Double click on a cell with code to activate that cell and work on it.

You should use this notebook step-wise:
1. Read the texts, sequentially.
2. The cells with code are numbered sequentially: `#1`, `#2`, .., so on. You **must execute the codes in that order only.**
3. To execute the code block in a cell, double-click on that cell to activate it. Then use `Ctrl + Enter` to execute the code in that cell.
4. Loading of packages may take a few seconds, depending upon your machine. Do not panic.
5. There is a small circle on the right-hand upper corner of Jupyter lab panel. That shows the status of the program. While the program is working, this circle will be filled and black. So, keep an eye on it. When the code in one cell is working, you should not try to run the code in another cell.

To run all the contents in the notebook use : `Run > Run All Cells`

**This GitHub repository may get updated. Please use the latest notebook.**



```


















