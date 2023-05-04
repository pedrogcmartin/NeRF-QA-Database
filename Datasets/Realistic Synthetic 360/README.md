This directory contains a dataset of synthetically rendered images that were used in "NeRF: Representing Scenes as
Neural Radiance Fields for View Synthesis".

Stats:
+ 4 Scenes
+ 100 Training images
+ 100 Validation images
+ 200 Test images
+ Images are 800x800

Structure:
  SCENE_NAME
    -train
      r_*.png
    -val
      r_*.png
    -test
      r_*.png
      r_*_depth_0000.png
      r_*_normal_0000.png
    transforms_train.json
    transforms_val.json
    transforms_test.json

Transform json details:
camera_angle_x: The FOV in x dimension
frames: List of dictionaries that contain the camera transform matrices for each image.

Attribution:
The renders are from modified blender models located on blendswap.com
drums by bryanajones (CC-BY): https://www.blendswap.com/blend/13383
ficus by Herberhold (CC-0): https://www.blendswap.com/blend/23125
lego by Heinzelnisse (CC-BY-NC): https://www.blendswap.com/blend/11490
ship by gregzaal (CC-BY-SA): https://www.blendswap.com/blend/8167
