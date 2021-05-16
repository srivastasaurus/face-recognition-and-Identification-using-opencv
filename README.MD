# INTRO

Face Recognition and Face identification in a video stream by using Face Recognition and opencv module . 

# Dependencies

Python, Opencv, Face-Recognition, numpy, cmake, dlib

# Install dependencies

> numpy :  $ sudo pip install numpy

# Install OpenCV

Follow the given steps

    [compiler] sudo apt-get install build-essential

    [required] sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev
    [optional] sudo apt-get install python-dev python-numpy libtbb2 libtbb-dev libjpeg-dev libpng-dev libtiff-dev libjasper-dev libdc1394-22-dev


    sudo mkdir opencv
    cd ~/opencv
    sudo git clone https://github.com/opencv/opencv.git
    sudo git clone https://github.com/opencv/opencv_contrib.git
    cd ./opencv
    sudo mkdir ./build
    cd ./build
    sudo cmake -D CMAKE_BUILD_TYPE=RELEASE \
        -D CMAKE_INSTALL_PREFIX=/usr/local \
        -D INSTALL_C_EXAMPLES=ON \
        -D INSTALL_PYTHON_EXAMPLES=ON \
        -D WITH_TBB=ON \
        -D WITH_V4L=ON \
        -D WITH_QT=ON \
        -D WITH_OPENGL=ON \
        -D OPENCV_EXTRA_MODULES_PATH=../../opencv_contrib/modules \
        -D BUILD_EXAMPLES=ON ..
    nproc
    make -j4
    sudo make install
    sudo sh -c 'echo "/usr/local/lib" >> /etc/ld.so.conf.d/opencv.conf'
    sudo ldconfig

# Install Face-Recognition

### Install 64 bit version of python from [here](https://www.python.org/)

