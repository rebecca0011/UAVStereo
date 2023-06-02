# UAVStereo
[UAVStereo](https://ieeexplore.ieee.org/document/10070843) is a multiple resolution dataset for stereo matching in UAV scenarios. The dataset provides multi-resolution and multi-scene image pairs to accommodate various sensors and environments.

## Download 
Baiduyun Link

Forest Eights(960*540px) [train](https://pan.baidu.com/s/1fhjedXMeZAnUBQJvM8tJ7w?pwd=1111)  [test](https://pan.baidu.com/s/1EnugvES-mYyAzC5F-cY4xw?pwd=1111)

Mining Eights(960*540px) [train](https://pan.baidu.com/s/1OuKa7U43N65b4pkYgUBK6g?pwd=1111)  [test](https://pan.baidu.com/s/1AbqIyS9OIKfwkSO4wFdxtA?pwd=1111)

Residential Eights(960*540px) [train](https://pan.baidu.com/s/1XyB2vxfTzlsnK-VhBiMljw?pwd=1111)  [test](https://pan.baidu.com/s/1qUiRYrMU7JhNauaItwQTPQ?pwd=1111)

Forest Quarters(1960*1080px) [train](https://pan.baidu.com/s/1itBzts02dpTfrf2SAlyMTA?pwd=1111)  [test](https://pan.baidu.com/s/1oUmyhYg7Sh_sTe4eus45WQ?pwd=1111)

Mining Quarters(1960*1080px) [train](https://pan.baidu.com/s/1gsYRExUY71UngWQodGsJMA?pwd=1111)  [test](https://pan.baidu.com/s/1GgVPgIyQJnFUqDo6Sh3FAQ?pwd=1111)

Residential Quarters(1960*1080px) [train](https://pan.baidu.com/s/19SNu7NMrMY0ojAxvMYug2w?pwd=1111)  [test](https://pan.baidu.com/s/12gH6x_nSBtp0-1mOLYLbRQ?pwd=1111)

Forest Half(3840*2160px) [train](https://pan.baidu.com/s/1D7k1INt-98wHLifK1PgwLA?pwd=1111)  [test](https://pan.baidu.com/s/1FLHMHbFJzBa0rOGUavg1dw?pwd=1111)

Mining Half(3840*2160px) [train](https://pan.baidu.com/s/1TGAYf3-Q6FLnhM6nQeyHSw?pwd=1111)  [test](https://pan.baidu.com/s/1MKJeLn6SBFqjyeHlyo4WwQ?pwd=1111)

Residential Half(3840*2160px) [train](https://pan.baidu.com/s/1HEPFht0mj1NszpCLe3eKOg?pwd=1111)  [test](https://pan.baidu.com/s/1RdNv2aTKafsYEBRxfYKG2g?pwd=1111)


[Whole UAVStereo](https://pan.baidu.com/s/1TVdsFE_V3LRfezuNmTzADQ?pwd=1111)



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
