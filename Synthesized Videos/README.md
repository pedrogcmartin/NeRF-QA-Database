The used terminology of video file names is:

[scene name]_[method name]_ mp4

or 

[scene name]_[method name]_ss2.mp4


where the scene name can be: drums, ficus, lego, and ship, for the synthetic scenes; or: m60, playground, train, and truck, for the real scenes. For the synthetic scenes the method's name can either be: dvgo, instantNGP, plenoxels, or tensorf (corresponding to the use of the DVGO, Instant-NGP, Plenoxels, and TensoRF methods); and for the real scenes: dvgo, mipnerf360, perfecto, or nerfplusplus (corresponding to the use of the DVGO, Mip-NeRF 360, Perfecto, and NeRF++ methods). For the synthetic scenes there can be a subsampling factor of 2 regarding the number of images used for the method's training. In that case, at the end of the file name there is an additional "_ss2" term. For example, when referring to the synthesized video of the lego synthetic scene with DVGO method and a subsampling factor of 2, the file name is: lego_dvgo_ss2.mp4. Otherwise, when referring to the synthesized video of the lego synthetic scene with DVGO method and no subsampling, the file name is: lego_dvgo.mp4.