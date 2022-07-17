# How-To-Install-TensorFlow-on-M1-Mac-
How To Install TensorFlow on M1 Mac 		  

You have to do the following steps:

•	Step 1: Xcode Command Line Tools
  If you already have the Xcode Command Line Tools installed, skip this step.
  Open a terminal and enter the following command:
  >>xcode-select --install
  
  After this command, the Tools will install on the Mac.

•	Step2: Install Miniforge
  Now you have to install Miniforge on your Mac.
  You can get it here:
  https://github.com/conda-forge/miniforge
  
  Miniforge enables installing python packages natively compiled for Apple Silicon.
  
  Or you can use miniconda https://docs.conda.io/en/latest/miniconda.html
  

•	Step3: Create a virtual environment with python3.8
  Now we need a virtual environment. To create one, we use the following command:
  >>conda create --name mlp python=3.8
  After that step, you have to enter the following command:
  
  >>conda activate mlp
  
•	Step4: Install Tensorflow 2.5 and its dependencies
  Now we can install Tensorflow.
  
  1. >>conda install -c apple tensorflow-deps
  2. >>pip install tensorflow-macos
  3. >>pip install tensorflow-metal

•	Step5: Install Jupyter Notebook, Pandas
  
  >>conda install -c conda-forge -y pandas jupyter

  
•	Step6: Open your Jupyter Notebook
  1.  >>conda activate mlp
  2.  >>jupyter notebook

If you want, you can run a benchmark check, to proof your System:

Follwoing the steps on https://github.com/apple/tensorflow_macos/issues/25
