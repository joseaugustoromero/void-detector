# void-detector working on windows

I forked the original 'void-detector' to make it running on windows, this project can be used to
detect voids in grocery store shelves. I took some pictures in a local grocery at my neighborhood here in Brazil to see if the void detector can work in differents places and with differents shelves. The technique behinde to turn this possible is the deep learning object detection algorithms like FPNSSD512 and YOLO

<img src="docs/local_brazilian_grocery.gif" width="50%">

The above are predictions from the images(the original images cand be foud in the imgs folder) that I took in the local grocery store.

### Dockerless on windows 10

`python demo.py IMAGE_DIR --dockerless`

Requirements:
- I make this repo working on Windows 10 with a gtx1070 NVIDIA GPU 
- [Anaconda 5, Python 3.6 version](https://www.anaconda.com/download/#windows)
- conda create -n void-detector python=3.6
- pip install opencv-python
- pip install requests
- pip install jupyter
- conda install pytorch torchvision cuda90 -c pytorch
- pip install tqdm

# Note
The original work was created by [MattKleinsmith](https://github.com/MattKleinsmith/void-detector), this repo is just a fork to test with some local images and to run on windows 10.