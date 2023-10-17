# Diabetic Retinopathy (DR) Detection with Machine Learning

- Input: Retinal fundus image
- Output: Diabetic Retinopathy grade
  - TODO on scale of
  - 0 - healthy,
  - 1 - NPDR (non proliferate),
  - 2 - PDR (proliferate)

Therefore this is a multi-class image classification problem. 

## Table of Contents

- [Prerequisites to set up](#prerequisites)
- [Tutorials](#tutorials)
- [Setting Up the Data Science Environment](#setting-up-the-data-science-environment)
- [Usage](#usage)
- [Contributing](#contributing)

---

## Prerequisites

Before you get started with the Diabetic Retinopathy Detection project, make sure you have the following prerequisites installed on your system:

- [Python](https://www.python.org/downloads/)
  - Verify your Python installation by running: `python3 --version`
- [Anaconda](https://www.anaconda.com/products/distribution)
  - Verify your Anaconda installation by running: `conda --version`
- [NVIDIA CUDA Toolkit](https://developer.nvidia.com/cuda-downloads)
  - Verify your CUDA installation by running: `nvcc --version`
- [Git](https://git-scm.com/download/win)
  - Verify your Git installation by running: `git --version`
- [Visual Studio Code (VSC)](https://code.visualstudio.com/download)
- [TensorFlow](https://www.tensorflow.org/install/source)
- [cuDNN](https://developer.nvidia.com/rdp/cudnn-archive)

**Note:** Please check the [TensorFlow compatibility page](https://www.tensorflow.org/install/source_windows#gpu) to ensure that your TensorFlow version is compatible with the installed CUDA version.
eg. 2023 project used the versions:
<img width="606" alt="image" src="https://github.com/yiyangjessieyu/Deep-Learning-Image-Classifier/assets/101782677/6da84553-2a2c-4a1f-ab64-eecdc62731f8">

## Tutorials

To help you get started with this project, you can refer to the following tutorials:

- [Getting Started with Python Deep Learning for Beginners](https://youtu.be/19LQRx78QVU?feature=shared)


## Setting Up the Data Science Environment

To set up your data science environment for the Diabetic Retinopathy Detection project, follow these steps:

1. Create a virtual environment and associate it with your Jupyter notebook. The example code below is used on Linux. For macOS or Windows options, refer to the [official Python documentation](https://docs.python.org/3/library/venv.html).

```bash
# Create a new virtual environment
python -m venv venv-seng402

# Activate the virtual environment
source venv-seng402/bin/activate

# Install ipykernel to allow attaching the virtual environment to Jupyter Notebook
pip install ipykernel

# Install the virtual environment as a Jupyter kernel
python -m ipykernel install --name=venv-seng402

# Check installed packages
pip list

# Alternatively, you can install the virtual environment as a Jupyter kernel using the following command:
python3 -m ipykernel install --user --name=venv-seng402
```

2. Install TensorFlow for deep learning in your activated virtual environment:

```bash
pip install tensorflow
```

3. Feel free to install any other dependencies you need in your virtual environment. If you encounter a "ModuleNotFoundError," install the missing module using `pip` in your virtual environment.

4. To delete unwanted environments from Jupyter, use the following command:

```bash
jupyter kernelspec uninstall [insert your unwanted kernel]
```

## Usage

You can now start using the Diabetic Retinopathy Detection project by running the provided Python scripts and notebooks in the order of: 
1. extract_data.ipynb
2. create_model.ipynb
3. predict_dr.ipynb

Refer to the project files for detailed usage instructions.


## Contributing

1. **Fork the Repository** to your GitHub account.

2. **Clone the Repository** to your local machine using `git clone`.

3. **Make Changes**. Implement your improvements or new features.

3. **Update Documention** for the README and/or any other files if your changes affect the project's setup or usage.

4. **Commit and Push** to your forked repository.


---

Thank you for contributing to this project to improve the detection of diabetic retinopath!


