# BossSensor
Hide your screen when your boss is approaching.

## Demo
The boss stands up. He is approaching.

![standup](https://github.com/Hironsan/BossSensor/blob/master/resource_for_readme/standup.jpg)

When he is approaching, the program fetches face images and classifies the image.
 
![approaching](https://github.com/Hironsan/BossSensor/blob/master/resource_for_readme/approach.jpg)

If the image is classified as the Boss, it will monitor changes.

![editor](https://github.com/Hironsan/BossSensor/blob/master/resource_for_readme/editor.jpg)

## Requirements

* WebCamera
* Python3.5
* OSX
* Anaconda
* Lots of images of your boss and other person image

Put images into [data/boss](https://github.com/Hironsan/BossSensor/tree/master/data/boss) and [data/other](https://github.com/Hironsan/BossSensor/tree/master/data/other).

## Usage
First, Train boss image.

```
$ python boss_train.py
```


Second, start BossSensor. 

```
$ python camera_reader.py
```

## Install
Install OpenCV, PyQt4, Anaconda.

```
conda create -n venv python=3.5
source activate venv
conda install -c https://conda.anaconda.org/menpo opencv3
conda install -c conda-forge tensorflow
pip install -r requirements.txt
```

Change Keras backend from Theano to TensorFlow. 

## Licence

[MIT](https://github.com/Hironsan/BossSensor/blob/master/LICENSE)

## Author

[Hironsan](https://github.com/Hironsan)


error

https://jingyan.baidu.com/article/6c67b1d6990aa12787bb1edd.html

```
INSTALL OPENCV

https://www.codingforentrepreneurs.com/blog/install-opencv-3-for-python-on-mac/

ln -s  /usr/local/Cellar/opencv/3.3.0_3/lib/python3.6/site-packages/cv2.cpython-36m-darwin.so   /Library/Frameworks/Python.framework/Versions/3.5/lib/python3.5/site-packages/cv2.so

install pyqt4 5

http://bomilanovich.com/blog/howto-install-pyqt-on-mac-with-python-3/

brew install qt

brew install sip --with-python3

pip3.5 install pyqt5

```
