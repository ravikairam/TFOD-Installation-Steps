# TFOD-Installation-Steps

TFOD: Pastebin Link
https://pastebin.com/YDgbqzTx

Steps 1:
Create a folder in Desktop name tfod:
steps 2:
Download first link from Pastebin doc (github Link)
https://github.com/tensorflow/models/tree/v1.13.0

Steps 3:
download pre trained model "Faster_rcnn_inception"
https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf1_detection_zoo.md

Steps 4:
Dataset & utils downloder
https://drive.google.com/file/d/12F5oGAuQg7qBM_267TCMt_rlorV-M7gf/view?usp=sharing

step 5:
Creating virtual env using conda
conda create -n your_env_name python=3.6

conda activate your_env_name

Steps 6: Install nacessary library using pip
pip install pillow lxml Cython contextlib2 jupyter matplotlib pandas opencv-python tensorflow==1.14.0

Steps 7:
extraxt your model file

rename only models

delete all files(not only research file)

Note: Research file is your parent folder

you should run your command in research folder

step 8:
set your file / Directory in research folder using anaconda

Steps 9: download tfod library 8:
write: python setup.py install ## (this is object detection library)

steup 10: convert proto file to py
conda install -c anaconda protobuf

Steps 11:
Inside research folder you have object_detection file then protos file then you have to convert all proto file into py

#windows protoc object_detection/protos/*.proto --python_out=.

#linux mac protoc object_detection/protos/*.proto --python_out=.

Steps 12:(!conda env list)
In object detection open you jupyter notebook

first set path write cd object_detection

( If you get any types of error in your jupyter notebook "ImportError: cannot import name 'string_int_label_map_pb2'")

OR

Copy your object detection ipynb file to research folder and open your jupyter notebook in research file & open your object detection notebook

Blog:
https://www.analyticsvidhya.com/blog/2020/04/build-your-own-object-detection-model-using-tensorflow-api/

