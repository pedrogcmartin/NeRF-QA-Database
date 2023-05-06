This directory contains a costumized version of the *Tanks and Temples* dataset - with real rendered images where the camera rotated 360 degrees around a point, or move around an interest region - that was used in:

K. Zhang, G. Riegler, N. Snavely, and V. Koltun, “NeRF++: Analyzing and Improving Neural Radiance Fields.” arXiv, Oct. 21, 2020. doi: 10.48550/arXiv.2010.07492.

Four scenes were considered from *Tanks and Temples*: *M60*, *Playground*, *Train*, and *Truck*.

Each scene folder contains:

+ The training images (277 for *M60*, 275 for *Playground*, 258 for *Train*, and 226 for *Truck*).
+ The training poses (one file per training image)
+ The intrinsics for each pose

The training images spatial resolution are: 1077×546 pixels for *M60*, 1008×548 pixels for *Playground*, 982×546 pixels for *Train*, and 980×546 pixels for *Truck*.

The training images, poses, and intrinsics are used as input for the NeRF based methods training.


# Attributions

The used images are from the *Tanks and Temples* dataset located on tanksandtemples.org
+ m60: https://drive.google.com/file/d/0B-ePgl6HF260dG9nTzZHdkRJblE/view?resourcekey=0-xjiyqBN2rRmYLnMBf-W_7w
+ playground: https://drive.google.com/file/d/0B-ePgl6HF260d0JoR2pWak9RbnM/view?resourcekey=0-zFg5ZGEBWA1USZ0pkqgUog
+ train: https://drive.google.com/file/d/0B-ePgl6HF260YUttRUI4U0xtS1E/view?resourcekey=0-fLiJMIqX8waMDBvg6XsEbw
+ truck: https://drive.google.com/file/d/0B-ePgl6HF260aVVZMzhSdVc5Njg/view?resourcekey=0-QYlGb_jIaM7Kq8NQQYZuyA
