# Setting up your system to run and modify lvv-ri-new

## Anaconda:
We recommend installing Python via the [Anaconda Distribution](https://www.anaconda.com/download). Be sure to use the "Python 3.8" version or higher. We will use the Conda Package Management System within the Anaconda Distribution. From the [documentation](https://conda.io/docs):
> Conda is an open source package management system and environment management system that runs on Windows, macOS and Linux. Conda quickly installs, runs and updates packages and their dependencies. Conda easily creates, saves, loads and switches between environments on your local computer.

After the installation run `python --version` in a terminal window (in "Anaconda Prompt" if you are using Windows). If the output show "Python 3.8.x" and "Anaconda" you are good to go.

## GitHub:
The code is hosted on the code-sharing platform GitHub (where you now are reading this). If you do not have a GitHub account already you should make one. We recommend that you are using this platform for you own projects. https://github.com/join.


## Install and test the lvv-ri-new environment:

After you have successfully installed Anaconda, go through the following steps (if you are using Windows, be at the "Anaconda Prompt").

### Install Git
```bash
conda install git
```
### Download the repository:
```bash
git clone https://github.com/mmiv-ml/lvv-ri-new
cd lvv-ri-new
```
### Configure the Python-environment:
```bash
conda env update
```

### Activate the environment:
```bash
conda activate lvv-ri-new
```

### Install a Jupyter kernel:
```bash
python -m ipykernel install --user --name lvv-ri-new --display-name "LVV-RI-NEW"
```

### Test your installation:
Go through the notebook `0.0-test.ipynb` in the `notebooks`-directory:
```bash
cd notebooks
jupyter notebook
```
You can also use [JupyterLab](https://github.com/jupyterlab/jupyterlab): `jupyter lab`.

## Update:
The code and environment might be updated to account for errors and improvements - the paper and the accompanying code (as accepted) can be regarded as a snapshot. To consider this, run the following commands:
* Update code: `git pull`
* Update environment:
```bash
conda activate lvv-ri-new
conda env update
```
