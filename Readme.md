# WebVision 1.0
This project preprocess the [WebVision 1.0 Dataset](https://data.vision.ee.ethz.ch/cvl/webvision/dataset2017.html) and gives a directory structure [ImageNet1k dataset](https://www.image-net.org/). 

### Dataset details

Check using ```find train/ -maxdepth 2 -type f | wc -l``` in terminal
 
- Number of train images - 2345405 
- Number of val images - 50000 (50 per class)

### Below is the final directory structure:
```
└── WebVision1.0
    ├── train
    |   ├── nxxxxxxxx
    |   ├── nxxxxxxxx
    |   └── ...
    |
    └── val
    |   ├── nxxxxxxxx
    |   ├── nxxxxxxxx
    |   └── ...
    |
    └── info
    |   ├── xxxx
    |   ├── xxx
    |   └── ...
    |
    └── create_WebVision_as_ImageNet.sh
    └── helper.py
    └── Readme.md
    └── Citation.cff
    └── LICENSE
```

Note Similar Processing can be done for the Flicker partition. Modify the create_WebVision_as_ImageNet.sh and helper.py.


## Instructions

1. Clone this repository
2. Navigate to the root of this project
3. Run the following command in your terminal/command prompt: 
 
    ```bash
    sh create_WebVision_as_ImageNet.sh
    ```


## Expected Terminal logs
```
----------------------------------------------------------------
Creating directory structure similar to ImageNet for training dataset
----------------------------------------------------------------
----------------------------------------------------------------
Creating directory structure similar to ImageNet for val dataset
----------------------------------------------------------------
----------------------------------------------------------------
Removing Redundant files.
----------------------------------------------------------------
----------------------------------------------------------------
WebVision Dataset 1.0 Processed!
----------------------------------------------------------------
```

# Conclusion

The project preprocess WebVision 1.0 Dataset and gives a directory structure similar to ImageNet.
The script automates the preprocessing and provides a directory structure for WebVision similar to ImageNet.




# Citation
Kindly cite the repository if you use the code. Thanks!

### APA
```
Kodge, S. (2024). WebVision1.0 [Computer software]. https://github.com/sangamesh-kodge/WebVision1.0
```

### Bibtex
```
@software{Kodge_WebVision1_0_2024,
author = {Kodge, Sangamesh},
month = feb,
title = {{WebVision1.0}},
url = {https://github.com/sangamesh-kodge/WebVision1.0},
year = {2024}
}
```
