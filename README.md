# AIR-Clothing-MA
This is a part of ETRI AIR project. The AIR-Clothing-MA(Multi Attributes) is a kind of mutli-attributes classifier for clothings and their multi attributes.

## Dependencies
-   python >= 3.6 
-   pytorch >= 1.2

-   RoiAlign 
    1. Download and install RoiAlign module for pytorch from [here](https://github.com/longcw/RoIAlign.pytorch)

## Installation
Recommend this procedure!!  (from ubuntu 18.04)
1. download & install cuda 10.2 toolkit 
 - [here](https://developer.nvidia.com/cuda-10.2-download-archive?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu&target_version=1804&target_type=debnetwork)
2. download & install anaconda python 3.7 version (Linux x86) 
 - [download](https://repo.anaconda.com/archive/Anaconda3-2020.02-Linux-x86_64.sh)
 - $ sh Anaconda3-2020.02-Linux-x86_64.sh
3. install pytorch
 - (base)$ conda install pytorch torchvision cudatoolkit=10.2 -c pytorch
4. install opencv, matplotlib
 - (base)$ pip install opencv-python, matplotlib
5. install RoIAlign
 - [RoIAlign](https://github.com/longcw/RoIAlign.pytorch)
 
## How to test the model

1.   Download yolo-v3 model from [here](https://drive.google.com/file/d/1yCz6pc6qHJD2Zcz8ldDmJ3NzE8wjaiT6/view?usp=sharing) and put in 'Air-Clothing-MA root directory'.  
2.   Downoad Clothing-MA model from [here](https://drive.google.com/file/d/1k3lvA96ZstbV4a_QtYTuohY79xg_nJYe/view?usp=sharing) and put in 'Air-Clothing-MA root directory'.
3.   Run 'file_demo.py' to run each image file demostration
4.   Run 'cam_demo.py' to run web-cam demostration

## LICENSE
This software is a part of AIR, and follows the [AIR License and Service Agreement](LICENSE.md).

## Acknowledgement
* This work was supported by the ICT R&D program of MSIP/IITP. [2017-0-00162, Development of Human-care Robot Technology for Aging Society]   
