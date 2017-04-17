# Keras_Win
Setting up Python, Tensorflow and Keras on Windows 10

## Install Python
Python can be downloaded from https://www.python.org/. This writeup assumes the use of Python 3.5 on Windows 10.

## Create a virtual environment
Create the *keras_env* virtual environment and activate it.
```
$ cd C:\Python\venvs
$ python -m venv keras_env
$ C:\Python\venvs\keras_env\Scripts\activate
```

## Install Python dependencies
Keras requires the following Python dependencies:
* Numpy (http://www.lfd.uci.edu/~gohlke/pythonlibs/#numpy)
* SciPy (http://www.lfd.uci.edu/~gohlke/pythonlibs/#scipy)
* HDF5/h5py (http://www.lfd.uci.edu/~gohlke/pythonlibs/#h5py)
* pyyaml ``` pip install pyyaml```
* Optional: cuDNN (Not used here)

## Install Tensorflow
In this case, we will install the CPU-only version of Tensorflow, through the native-pip interface (https://www.tensorflow.org/install/install_windows).
* From the virtual environment: ```pip install --upgrade tensorflow```
* Test proper function of TF. The following import of the TF package in python should not produce errors:
```
(keras_env) $ python
(python) >>> import tensorflow
```

## Install Keras
* From virtual environment: ```pip install keras```
* Test proper installation and integration with TF. Importing keras should produce the following message about tensorflow backend:
```
(keras_env) $ python
(python) >>> import keras
(python) Using tensorflow backend.
