# Self Driving Car

In this project, I trained a self-driving car model using behavioral cloning, where the model learns to imitate human driving behavior from recorded data. The trained model can then be used to drive the car autonomously within the Udacity simulator environment.


## Overview

I used Udacity's [self driving car simulator](https://github.com/udacity/self-driving-car-sim) as a testbed for training an autonomous car. 

## Dependencies

You can install all dependencies by running one of the following commands

You need a [anaconda](https://www.continuum.io/downloads) or [miniconda](https://conda.io/miniconda.html) to use the environment setting.

```python
# Use TensorFlow without GPU
conda env create -f environments.yml 

# Use TensorFlow with GPU
conda env create -f environment-gpu.yml
```

Or you can manually install the required libraries (see the contents of the environemnt*.yml files) using pip.

### Tech Stack

  * Python
  * Keras (for neural network modeling)
  * OpenCV (for image processing)
  * NumPy, Pandas (for data manipulation)
  * Flask (for web server)
  * SocketIO (for communication with the Udacity simulator)
  * Udacity Self-Driving Car Simulator


### Run the pretrained model

Start up [the Udacity self-driving simulator](https://github.com/udacity/self-driving-car-sim), choose a scene and press the Autonomous Mode button.  Then, run the model as follows:

```python
python drive.py model.h5
```

### To train the model

You'll need the data folder which contains the training images.

```python
python model.py
```

This will generate a file `model-<epoch>.h5` whenever the performance in the epoch is better than the previous best.  For example, the first epoch will generate a file called `model-000.h5`.






