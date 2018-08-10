# NASNet

This repo contains keras.applications folder in which is located nasnet.py file. That file makes NASNet architecture, both Large and Mobile, and loads weights gotten from the ImageNet dataset. 

In order to change number of input channels, from 3 to 20, I needed to change weights file, speficically weights of the first convolutional layer. Changed file is also contained within this repo. After that, when model made using nasnet.NASNetMobile() is ready to receive optical flow images.

After this I was able to replace VGG-16 architecture from temporalneturfd.py with NASNetMobile. For feature extracion part I kept all the layers, apart from the last Dense layer.