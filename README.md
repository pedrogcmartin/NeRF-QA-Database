# NeRF-QA Database

This repository contains a database with NeRF test sequences of Tanks&Temples and NeRF Synthetic datasets generanted by DVGO, Instant-NGP, Mip-NeRF 360, Nerfacto, NeRF++, and Plenoxels methods. The results of a subjective assessment study are also provided.

The subjective assessment of novel view synthesis with Neural Radiance Fields (NeRF) based methods was conducted using eight visual scenes taken from two popular datasets, namely Tanks and Temples [1] and Realistic Synthetic 360º [2], where the former resulted from real-world 360 degrees captures of large scenarios, and the latter was obtained with Blender [3]. The selected videos from Tanks and Temples were M60, playground, train, and truck. This dataset was used as processed in [4], where the number of training frames are equal to 277, 275, 258, and 226 frames, respectively, having spatial resolutions of 1077×546, 1008×548, 982×546, and 980×546 pixels. The scenes selected from Realistic Synthetic 360º were drums, ficus, lego, and ship, having all 100 training frames with spatial resolutions of 800×800 pixels. For the subjective test purpose, the spatial resolutions of the real scenes were uniformized with a downsampling to 960×540 pixels, followed by a cropping to 928×522 pixels. For generating the reference videos, the video duration was set to 10 s for real scenes, and to 6 s for synthetic scenes. In every case, the rendered camera poses do not coincide with the training poses. 

The NeRF methods selected for the real scenes were DVGO, Mip-NeRF 360, Nerfacto, NeRF++ [5,6,7,8]. For the synthetic scenes, the selected synthesis methods were DVGO, Instant-NGP, Plenoxels, and TensoRF [5,9,10,11]. The selected datasets have already been used in published works, enabling the validation of the herein generated synthesized videos, by comparison of the obtained objective quality metrics values (using PSNR and SSIM) with the values reported on those works. Lastly, the synthetic scenes were also synthesized for the case where a subsampling with a factor of 2 was applied to the training set, seeking synthesized video qualities covering the lowest qualities range.

The Double Stimulus Continous Quality Scale (DSCQS) was selected as an evaluation method. A total of 48 pairs of stimulus (32 synthesized synthetic videos + 16 synthesized real videos, together with the respective original videos) were assessed. After the test, the resulting scores were processed according to [18] to obtain Differential Mean Opinion Score (DMOS) values for each synthesized video. More details about the subjective assessment procedure can be found in [12].

The NQ-NeRF database repository is organized as follows: the datasets used to generate the synthesized videos are in the "datasets" folder; the reference and synthesized videos used on the subjective test are in the "Reference Videos" and "Synthesized Videos" folders; and the "DMOS.xlsx" file has the subjective test DMOS results.

# References

[1]

[2]

[3]

[4]

[5]

[6]

[7]

[8]

[9]

[10]

[11]

[12]