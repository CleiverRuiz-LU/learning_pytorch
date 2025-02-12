# Setting Up a Conda Environment for Python Development
This guide will walk you through the process of setting up your Conda environment for learning Python, including the installation of necessary packages.

## Step 1: Install Anaconda or Miniconda

First, you need to have Anaconda or Miniconda installed. Anaconda includes Conda, Python, and a bunch of pre-installed packages, which is very convenient for beginners. Miniconda has fewer pre-installed packages but is lighter and quicker to install.

-  **Anaconda:** Download from [Anaconda.com](https://www.anaconda.com/products/individual).
-  **Miniconda:** Download from [Miniconda Official Docs](https://docs.conda.io/en/latest/miniconda.html).

## Step 2: Create a New Conda Environment

Once Anaconda or Miniconda is installed, you can create a new environment specifically for your Python tutorials.

1. Open your terminal (or Anaconda Prompt if you are on Windows).
2. Create a new environment by running:
   ```bash
   conda create --name Learning_PyTorch python=3.10
   ```
   Replace `Learning_PyTorch` with whatever name you wish to give your environment, and `3.10` with the version of Python you want to use.

## Step 3: Activate Your Environment

Before you start installing packages or running Python, you need to activate the environment you just created:
```bash
conda activate Learning_PyTorch
```

## Step 4: Install Necessary Packages

With your environment activated, you can now install any packages you need using Conda. 
```bash
pip install -r requirements.txt
```

Ensure your `requirements.txt` file includes the corrected package versions as follows:
```
torchao==0.8.0 # was originally 0.5.0
torchrl==0.3.1 # was originally 0.6.0
tensordict==0.3.2 # was originally 0.6.0
torch==2.2.2 # was originally 2.6
```
There were some issues when installing through pip; therefore, the following corrections above were necessary to ensure all packages could be installed.

## Step 5: Verify Your Installation

Check that the required packages are installed in your Conda environment:
```bash
conda list
```

This command will display all the packages installed in your environment, allowing you to verify that everything is set up correctly.
