# UAVStereo
[UAVStereo](https://ieeexplore.ieee.org/document/10070843) is a multiple resolution dataset for stereo matching in UAV scenarios. The dataset provides multi-resolution and multi-scene image pairs to accommodate various sensors and environments.

## Download 
Baiduyun Link
[Whole UAVStereo](https://pan.baidu.com/s/1TVdsFE_V3LRfezuNmTzADQ?pwd=1111)

Google Drive
Forest Eights(960*540px) [train](https://pan.baidu.com/s/1fhjedXMeZAnUBQJvM8tJ7w?pwd=1111)  [test](https://pan.baidu.com/s/1EnugvES-mYyAzC5F-cY4xw?pwd=1111)

Mining Eights(960*540px) [train](https://pan.baidu.com/s/1OuKa7U43N65b4pkYgUBK6g?pwd=1111)  [test](https://pan.baidu.com/s/1AbqIyS9OIKfwkSO4wFdxtA?pwd=1111)

Residential Eights(960*540px) [train](https://drive.google.com/file/d/1YeqmSC3sLbClXFRjW6FWw8mIKyoKGp25/view?usp=sharing)  [test](https://drive.google.com/file/d/1k0r7mmux7zLdZ5LPIdBzGJ9xXEQ0mN3_/view?usp=sharing)



## Scenes

Three different scenarios were included in the UAVStereo dataset: residential land, forest, and mining areas.

The residential area contains dense and regular tall buildings, flat roadways, and other urban scene features. This area provides an urban scene with disparity saltation, such as buildings. 

<img src="Scene/03.PNG" width="60%">


The forest area contains high-coverage trees, several houses, and other field scene components. This region has textureless and repeated-texture images, which presents difficulties for stereo-matching algorithms.

<img src="Scene/01.PNG" width="60%">

The mining zone is composed of agriculture, low structures, and bare ground, which contain a continuous variation of disparity.

<img src="Scene/02.PNG" width="60%">

These three areas are representative areas for UAV Earth observations and can represent different disparity distributions.

## Samples

<img src="Scene/04.png" width="80%">

## Dataset Structure

```

Data root
|-Forest
|-Mining
|-Residential
    |--train
    |--test
        |---Eights(960*540px)
        |---Quarters(1960*1080px)
        |---Half(3840*2160px)
            |----**-Baseline-15
            |----**-Baseline-16
             ...
            |----**-Baseline-35
                      |-----ImageLeft
                              |------000*_L.png
                              ...
                      |-----ImageRight
                              |------000*_R.png
                              ...
                      |-----DispLeft
                              |------000*_L.pfm
                              ...
                      |-----DispRight
                              |------000*_R.pfm
                              ...
 
```
