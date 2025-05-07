# tmmax-workshop

This workshop is given as part of the graduate-level Thin Film Coatings (given by Prof. Dr. Esra Zayim) course at Istanbul Technical University by Bahrem Serhat Danis. It is designed to introduce students to the `tmmax` Python library, which facilitates fast and efficient simulations of thin film materials.

In this workshop, you will how to simulate thin film materials and their properties using tmmax. We will guide you step-by-step through setting up your environment, installing the necessary tools, and running your first simulations.

# Prerequisites

Before starting the workshop, ensure you have Python installed on your system. If you don’t have Python, please follow the steps below to install it.

## Step 1: Installing Python

To install Python, we recommend using Anaconda as it simplifies the process of managing Python environments and dependencies.

For Windows, Mac, and Linux:

1. Download Anaconda:
   - Go to the Anaconda Downloads page (https://www.anaconda.com/products/individual) and select the appropriate version of Anaconda for your operating system (Windows, Mac, or Linux).
   - Follow the installation instructions for your OS.

2. Install Anaconda:
   - On Windows, run the downloaded .exe file.
   - On Mac and Linux, follow the terminal instructions after downloading the appropriate .pkg or .sh file.

## Step 2: Setting Up the Virtual Environment

After installing Anaconda, you can create a virtual environment to isolate your Python packages for this workshop.

1. Open the Anaconda Prompt or Terminal:
   - Windows: Open the Anaconda Prompt.
   - Mac/Linux: Open the Terminal.

2. Create a Virtual Environment:
   Run the following command to create a virtual environment for the tmmax library:

  ```bash
  conda create --name tmmax_env python=3.9
  ```
3. Activate the Virtual Environment:

  After creating the virtual environment, activate it with the following command:
  
  ```bash
  conda activate tmmax_env
  ```

## Step 3: Installing the tmmax Library

With the virtual environment activated, you can now install tmmax using pip.

1. Install tmmax:

  ```bash
  pip install tmmax
  ```

## Step 4: Setting Up Jupyter Notebook Kernel

In this step, we’ll set up Jupyter Notebook to use the virtual environment (tmmax_env) as a kernel. Jupyter Notebooks allow you to run and interact with Python code directly from your browser.

1. Install Jupyter Notebook (if not already installed):

  ```bash
  conda install jupyter
  ```

2. Install IPython Kernel:

  This will allow the Jupyter Notebook to recognize your virtual environment.
  
  ```bash
   pip install ipykernel
  ```

3. Create a Jupyter Kernel for the Virtual Environment:

  Now, register the virtual environment as a Jupyter kernel:
  
  ```bash
  python -m ipykernel install --user --name=tmmax_env --display-name "Python (tmmax_env)"
  ```

## Step 5: Launching Jupyter Notebook

Now that your environment is set up, you can launch Jupyter Notebook and start working with tmmax in the notebook interface.

1. Start Jupyter Notebook:

  Run the following command to start Jupyter Notebook:
  
  ```bash
  jupyter notebook
  ```
  
  This will open Jupyter Notebook in your web browser.

2. Select the Kernel:

  Once the Jupyter Notebook interface is open, create a new notebook:
  
  - Click on New in the top right corner.
  
  - Select Python (tmmax_env) from the dropdown menu to use the virtual environment kernel.
