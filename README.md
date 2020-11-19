# Dog-Breed-Classifier

Udacity DSND Project on creating a dog breed image classifier with keras.

## Overview

This project is part of Udacity's Data Science Nanodegree. The aim of the project is to create an application that is able to identify a breed of dog if given a photo or image as input. If the photo or image contains a human face, then the application will return the breed of dog that most resembles this person. The final model for identifying dog breeds achieved an **84.2%** accuracy level on the testing dataset. A post of this application can be found via this [LINK](https://dyushu.medium.com/dog-breed-classifier-73f1ce7f607a).


## Repository Contents

The main file in the repository is the dog_app.ipynb, which is the Jupyter notebook containing the process used to create our algorithm and model used to predict the dog breed. A report.html is also included in this repository.

 - The `haarcascades` folder holds the xml file for use with the OpenCv face detector class that is used in the notebook. 
 - The `images folder` contains the images used to test the predictions of the final model in the notebook. 
 - The `my_images` folder contains the sample images used to test the algorithm.

### Instructions

The instructions are from this [LINK](https://github.com/udacity/dog-project.git)

1. Clone the repository and navigate to the downloaded folder.
```
git clone https://github.com/udacity/dog-project.git
cd dog-project
```

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`.

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder.

4. Donwload the [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) for the dog dataset.  Place it in the repo, at location `path/to/dog-project/bottleneck_features`.

5. (Optional) __If you plan to install TensorFlow with GPU support on your local machine__, follow [the guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.  If you are using an EC2 GPU instance, you can skip this step.

6. (Optional) **If you are running the project on your local machine (and not using AWS)**, create (and activate) a new environment.

	- __Linux__ (to install with __GPU support__, change `requirements/dog-linux.yml` to `requirements/dog-linux-gpu.yml`):
	```
	conda env create -f requirements/dog-linux.yml
	source activate dog-project
	```
	- __Mac__ (to install with __GPU support__, change `requirements/dog-mac.yml` to `requirements/dog-mac-gpu.yml`):
	```
	conda env create -f requirements/dog-mac.yml
	source activate dog-project
	```
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/dog-windows.yml` to `requirements/dog-windows-gpu.yml`):
	```
	conda env create -f requirements/dog-windows.yml
	activate dog-project
	```

7. (Optional) **If you are running the project on your local machine (and not using AWS)** and Step 6 throws errors, try this __alternative__ step to create your environment.

	- __Linux__ or __Mac__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`):
	```
	conda create --name dog-project python=3.5
	source activate dog-project
	pip install -r requirements/requirements.txt
	```
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`):
	```
	conda create --name dog-project python=3.5
	activate dog-project
	pip install -r requirements/requirements.txt
	```

8. (Optional) **If you are using AWS**, install Tensorflow.
```
sudo python3 -m pip install -r requirements/requirements-gpu.txt
```

9. Switch [Keras backend](https://keras.io/backend/) to TensorFlow.
	- __Linux__ or __Mac__:
		```
		KERAS_BACKEND=tensorflow python -c "from keras import backend"
		```
	- __Windows__:
		```
		set KERAS_BACKEND=tensorflow
		python -c "from keras import backend"
		```

10. (Optional) **If you are running the project on your local machine (and not using AWS)**, create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `dog-project` environment.
```
python -m ipykernel install --user --name dog-project --display-name "dog-project"
```

11. Open the notebook.
```
jupyter notebook dog_app.ipynb
```

12. (Optional) **If you are running the project on your local machine (and not using AWS)**, before running code, change the kernel to match the dog-project environment by using the drop-down menu (**Kernel > Change kernel > dog-project**). Then, follow the instructions in the notebook.

__NOTE:__ While some code has already been implemented to get you started, you will need to implement additional functionality to successfully answer all of the questions included in the notebook. __Unless requested, do not modify code that has already been included.__

## Acknowledgements

Many of my ideas for this project have been taken from the lessons on the Udacity website and supporting github repositories. 
