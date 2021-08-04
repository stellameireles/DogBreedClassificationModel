# Dog-Breed-Classification
Udacity DataScience NanoDegree Capstone Project

### Table of Contents

1. [Instructions](#instructions)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Instructions <a name="instructions"></a>



1. Clone the repository and navigate to the downloaded folder.
```	
git clone https://github.com/stellameireles/DogBreedClassificationModel
cd 
```

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`. 

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 

4. 
- Donwload the [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) for the dog dataset.  Place it in the repo, at location `path/to/dog-project/bottleneck_features`.

- Donwload the [Inception-V3 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogInceptionV3Data.npz) for the dog dataset.  Place it in the repo, at location `path/to/dog-project/bottleneck_features`.


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


## Project Motivation<a name="motivation"></a>

This project provides a Dog Breed Identification using CNN - Convolutional Neureal Networks to extract features from the training datasets and predict if the image is of a human or a dog, and also give the dog breed most similar to the image. 

## File Descriptions <a name="files"></a>

1) Dog Image Dataset- 133 total dog categories and 8351 total dog images in the dog dataset. I

2) Human Face Image Dataset- 13233 total human images.



###### haarcascades

| - haarcascade_frontalface_alt.xml

###### images

| - American_water_spaniel_00648.jpg

| - Brittany_02625.jpg

| - Curly-coated_retriever_03896.jpg

| - Labrador_retriever_06449.jpg

| - Labrador_retriever_06455.jpg

| - Labrador_retriever_06457.jpg

| - Welsh_springer_spaniel_08203.jpg

| - sample_cnn.png

| - sample_dog_output.png

| - sample_human_2.png

| - sample_human_output.png

###### requirements

|- dog-linux-gpu.yml

|- dog-linux.yml

|- dog-mac-gpu.yml

|- dog-mac.yml

|- dog-windows-gpu.yml

|- dog-windows.yml

|- requirements-gpu.txt

|- requirements.txt

###### saved_models

|- weights.best.Inception.hdf5

|- weights.best.InceptionV3.hdf5

|- weights.best.VGG16.hdf5

|- weights.best.from_scratch.hdf5

###### .DS_Store

###### CODEOWNERS

###### LICENSE.txt

###### README.md

###### dog_app.ipynb

###### extract_bottleneck_features.py

## Results<a name="results"></a>

A post about the project can be found here [here]. https://stellameireles.medium.com/if-you-were-a-dog-2195bf8b9d11

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

This is a capstone project by the Data Scientist course from Udacity.
