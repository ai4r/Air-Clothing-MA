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
 - (base)$ pip install opencv-python matplotlib
5. install RoIAlign
 - [RoIAlign](https://github.com/longcw/RoIAlign.pytorch)
 
## How to test the model

1.   Download yolo-v3 model from [here](https://drive.google.com/file/d/1yCz6pc6qHJD2Zcz8ldDmJ3NzE8wjaiT6/view?usp=sharing) and put in 'Air-Clothing-MA root directory'.  
2.   Downoad Clothing-MA model from [here](https://drive.google.com/file/d/1k3lvA96ZstbV4a_QtYTuohY79xg_nJYe/view?usp=sharing) and put in 'Air-Clothing-MA root directory'.
3.   Run 'file_demo.py' to run each image file demostration
4.   Run 'cam_demo.py' to run web-cam demostration

## Clothing multi-attributes definition

<span class="c9"></span>

<a id="t.a6c6345e9a73b3ad660c800fb95cf5cfd611401e"></a><a id="t.0"></a>

<table class="c11">

<tbody>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">1</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">2</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">3</span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0">4</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">5</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0">6</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">7</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0">8</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">9</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">10</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">11</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">12</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">13</span>

</td>

</tr>

<tr class="c10">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">GT values</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">Top color(14)</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">Top pattern(6)</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">Top gender(2)</span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0">Top season(4)</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">Top type(7)</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0">Top sleeves(3)</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">Bottom color(14)</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0">Bottom pattern(6)</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">Bottom gender(2)</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">Bottom season(4)</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">Bottom length(2)</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">Bottom type(2)</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">leg pose(3)</span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">0</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">null</span>

</td>

</tr>

<tr class="c10">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">1</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">white</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">plain</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">man</span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0">spring</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">shirt</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0">short sleeves</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">white</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0">plain</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">man</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">spring</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">short pants</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">pants</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">standing</span>

</td>

</tr>

<tr class="c10">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">2</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">black</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">checker</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">woman</span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0">summer</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">jumper</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0">long sleeves</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">black</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0">checker</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">woman</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">summer</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">long pants</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">skirt</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">sitting</span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">3</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">gray</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">dotted</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0">autunm</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">jacket</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0">no sleeves</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">gray</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0">dotted</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">autunm</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">lying</span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">4</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">pink</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">floral</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0">winter</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">vest</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">pink</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0">floral</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">winter</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">5</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">red</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">striped</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">parka</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">red</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0">striped</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">6</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">green</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0">mixed</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">coat</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">green</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0">mixed</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">7</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">blue</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">dress</span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">blue</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">8</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">brown</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">brown</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">9</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">navy</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">navy</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">10</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">beige</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">beige</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">11</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">yellow</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">yellow</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">12</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">purple</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">purple</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">13</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">orange</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">orange</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

<tr class="c8">

<td class="c2" colspan="1" rowspan="1">

<span class="c0">14</span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">mixed</span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c5" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c7" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0">mixed</span>

</td>

<td class="c3" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c1" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

<td class="c2" colspan="1" rowspan="1">

<span class="c0"></span>

</td>

</tr>

</tbody>

</table>

<span class="c9"></span>		

## Example : Online Demostration - image 
<img src="example1.png" width="50%" height="50%" title="px(픽셀) 크기 설정" alt="Demo_image"></img>
## LICENSE
This software is a part of AIR, and follows the [AIR License and Service Agreement](LICENSE.md).

## Acknowledgement
* This work was supported by the ICT R&D program of MSIP/IITP. [2017-0-00162, Development of Human-care Robot Technology for Aging Society]   
