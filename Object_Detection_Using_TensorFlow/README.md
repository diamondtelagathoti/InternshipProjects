# Object Detection Using TensorFlow  

This repository contains the works which I have done using TensorFlow Object Detection API. Before running the code, you need to first install tensorflow and all its dependecies.  

### Installation ###

```System: Ubuntu 16.04 LTS or later```  

``pip`` is a python package manager used for installing all the modules to your system, if ``pip`` is not installed, then run the following command before insalling dependecies:  

```
For python 2.7:
	sudo apt-get -y install python-pip python-dev build-essential  
	sudo pip install --upgrade pip  
For python 3:  
	sudo apt-get -y install python3-pip  
	pip3 -version (For checking the version of pip3)  
For python 2.7:  
	sudo pip install -r dependencies.txt  
For python 3:  
	sudo pip3 install -r dependencies.txt  
Note: dependencies.txt file contains all the dependencies in order to run tensorflow on your system.  
```
After installing the tensorflow 1.5.0, and all the dependencies, you need to run the following commands,
	``sudo apt-get install python3-tk (For installing tkinter library)``  

In python interpreter, run the following cmds:
```
import tensorflow as tf
print(tf.__version__) #print the version of tensorflow installed in your system.
```
After sucessfully installing tensorFlow, issue the following cmds to install tensorFlow Object Detection API  

#### Protobuf Compilation: ####  
The Tensorflow Object Detection API uses Protobufs to configure model and training parameters.  
Before the framework can be used, the Protobuf libraries must be compiled.  

This should be done by running the following cmd from the tensorflow/models/research/ directory:  
``protoc object_detection/protos/*.proto --python_out=.``  

Basically the above cmd, creates .ipynb file for every .proto file in the protos directory in object detection folder  
``tensorflow/models/research/object detection/protos`` 

Adding libraries to ``PYTHONPATH``  
When running locally, the ``tensorflow/models/research/`` and slim directories should be appended to ``PYTHONPATH.``  

This can be done by running the following from ``tensorflow/models/research/:``  

``export PYTHONPATH=$PYTHONPATH:`pwd`:`pwd`/slim``  

Note: This command needs to run from every new terminal you start.  

If you wish to avoid running this manually, you can add the above as a new line to the end of your ~/.bashrc file.  
E.g. ``sudo nano ~/.bashrc`` and then add the above command at the end of the file.  

#### Testing the installation: ####  
Test whether you have correctly installed the Tensorflow Object Detection API by running the following command:  
``python3 object_detection/builders/model_builder_test.py``

If the above cmd executes sucessfully, means you have installed TensorFlow Object Detection API sucessfully.  

I am using ``OpenCV`` for implementing the object detection in real-time, you need to install ``OpenCV``.  
Refer the link for installing [OpenCV] (https://www.pyimagesearch.com/2016/10/24/ubuntu-16-04-how-to-install-opencv/)  
Now, you can run the code sucessfully.  

