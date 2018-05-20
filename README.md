# Caffe

This caffe is adapted to meet the requirement of fine-grained aerial image recognition tasks
(e.g. road and building segmentation and classification). 

This repo is verified on [bvlc/caffe](https://hub.docker.com/r/bvlc/caffe) docker image; just simply deploy this repo into `/opt/caffe` of the docker container. The brief steps to compile this repo are

- In terminal, run ```docker pull bvlc/caffe:cpu```
- Start docker with a local folder mounted: ```docker run -it --name caffe_test -v /path/to/local/folder:/dvol bvlc/caffe:cpu```
- Copy the entire repo into ```/path/to/local/folder``` and then into ```/opt/caffe``` overwritting folders.
- Install libmatio: ```sudo apt-get update && sudo apt-get install libmatio-dev```
- In folder ```/opt/caffe/build```, run ```make all -j4``` and wait till it finishes
- Test the installation using ...


