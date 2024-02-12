This directory contains a costumized version of the *Realistic Synthetic 360º* dataset - with synthetically rendered images where the camera rotated 360 degrees around a point, or move around an interest region - that was used in:

B. Mildenhall, P. P. Srinivasan, M. Tancik, J. T. Barron, R. Ramamoorthi, and R. Ng, “NeRF: representing scenes as neural radiance fields for view synthesis,” in Commun. ACM, vol. 65, no. 1, pp. 99–106, Dec. 2021, doi: 10.1145/3503250.

Four scenes were considered from *Realistic Synthetic 360º*: *Drums*, *Ficus*, *Lego*, and *Ship*.

Each scene folder contains:

+ 100 Traning images (with spatial resolution of 800×800 pixels)
+ 100 Training poses (within a transforms_train.json file)

The training images and poses are used as input for the NeRF based methods training. The json file also stores the intrinsics information regarding the camera poses for each training image.

# Attributions

The renders are from modified blender models located on blendswap.com
+ drums by bryanajones (CC-BY): https://www.blendswap.com/blend/13383
+ ficus by Herberhold (CC-0): https://www.blendswap.com/blend/23125
+ lego by Heinzelnisse (CC-BY-NC): https://www.blendswap.com/blend/11490
+ ship by gregzaal (CC-BY-SA): https://www.blendswap.com/blend/8167
