This directory contains a dataset of real images that were used in "NeRF++: Analyzing and Improving Neural Radiance Fields".

Stats:
+ The 4 Scenes are *M60*, *Playground*, *Train*, and *Truck*.
+ Number of raining images are 277, 275, 258, and 226 images.
+ 1 Camera path per scene.
+ Images are 1077×546, 1008×548, 982×546, and 980×546 pixels.

Structure:
  SCENE_NAME
    -train
      -intrinsics
        *.png
      -pose
        *.png
      -rgb
        *.png
    -camera_path
      -intrinsics
        *.png
      -pose
        *.png

Attribution:
The used images are from the *Tanks and Temples* dataset located on tanksandtemples.org.