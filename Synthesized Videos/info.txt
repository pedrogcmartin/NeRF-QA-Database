The used terminology of video file names is the following:

[scene name]_[method name]_ss[subsampling factor].mp4

where the scene name can be: drums, ficus, lego, and ship, for the synthetic scenes; or: m60, playground, train, and truck, for the real scenes. For the synthetic scenes the method's name can either be: dvgo, instantNGP, plenoxels, or tensorf (corresponding to the use of the DVGO, Instant-NGP, Plenoxels, and TensoRF methods); and for the real scenes: dvgo, mipnerf360, perfecto, or nerfplusplus (corresponding to the use of the DVGO, Mip-NeRF 360, Perfecto, and NeRF++ methods). For the synthetic scenes the subsampling factor of the number of images used for the method's training can either be 1 or 2; and for the real scenes the subsampling factor is always equal to 1. 

For example, when referring to the synthesized video of the lego synthetic scene with DVGO method and a subsampling factor of 1 the video file name is: lego_dvgo_ss1.mp4.