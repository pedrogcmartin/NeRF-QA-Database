# NeRF-QA Database

The Neural Radiance Fields-Quality Assessment (NeRF-QA) database contains: a dataset (in the "Datasets" folder) with eight, real and synthetic, visual scenes (in the "Tanks and Temples" and "Realistic Synthetic 360" folders, respectively) that are used to train seven NeRF based methods (nameley: DVGO, Instant-NGP, Mip-NeRF 360, Nerfacto, NeRF++, Plenoxels, and TensoRF [1,2,3,4,5,6,7]); the corresponding visual scenes reference videos (in the "Reference Videos" folder), with durations of 10 s and 6 s, for real and synthetics scenes, respectively; based on the trained methods, for each scene, the synthesized videos are also generated for the same test time interval of the reference videos and stored herein (in the "Synthesized Videos" folder); and, at last, the results of a subjective study comparing the qualities of the reference and synthesized videos by a group of 20 participants (in the "DMOS.xlsx" file).

The subjective assessment of synthesized videos was conducted using eight visual scenes taken from two popular datasets, namely *Tanks and Temples* [8] and *Realistic Synthetic 360º* [9], where the former resulted from real-world 360 degrees captures of large scenarios, and the latter was obtained with *Blender* [10]. The selected videos from *Tanks and Temples* were *M60*, *playground*, *train*, and *truck*. This dataset was used as processed in [4], where the number of training frames are equal to 277, 275, 258, and 226 frames, respectively, having spatial resolutions of 1077×546, 1008×548, 982×546, and 980×546 pixels. The scenes selected from *Realistic Synthetic 360º* were *drums*, *ficus*, *lego*, and *ship*, having all 100 training frames with spatial resolutions of 800×800 pixels. For the subjective test purpose, the spatial resolutions of the real scenes were uniformized with a downsampling to 960×540 pixels, followed by a cropping to 928×522 pixels. For generating the reference videos, the video duration was set to 10 s for real scenes, and to 6 s for synthetic scenes. In every case, the rendered camera poses do not coincide with the training poses. 

The NeRF methods selected for the real scenes were DVGO, Mip-NeRF 360, Nerfacto, NeRF++ [1,3,4,5]. For the synthetic scenes, the selected synthesis methods were DVGO, Instant-NGP, Plenoxels, and TensoRF [1,2,6,7]. The selected datasets have already been used in published works, enabling the validation of the herein generated synthesized videos, by comparison of the obtained objective quality metrics values (using PSNR and SSIM) with the values reported on those works. Lastly, the synthetic scenes were also synthesized for the case where a subsampling with a factor of 2 was applied to the training set, seeking synthesized video qualities covering the lowest qualities range.

The Double Stimulus Continous Quality Scale (DSCQS) was selected as an evaluation method. A total of 48 pairs of stimulus (32 synthesized synthetic videos + 16 synthesized real videos, together with the respective original videos) were assessed. After the test, the resulting scores were processed according to [11] to obtain Differential Mean Opinion Score (DMOS) values for each synthesized video. More details about the subjective assessment procedure can be found in [11].

# References

[1] C. Sun, M. Sun, and H.-T. Chen, “Direct Voxel Grid Optimization: Super-Fast Convergence for Radiance Fields Reconstruction,” in Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, 2022, pp. 5459–5469.

[2] T. Müller, A. Evans, C. Schied, and A. Keller, “Instant neural graphics primitives with a multiresolution hash encoding,” in ACM Trans. Graph., vol. 41, no. 4, p. 102:1-102:15, Jul. 2022, doi: 10.1145/3528223.3530127.

[3] J. T. Barron, B. Mildenhall, D. Verbin, P. P. Srinivasan, and P. Hedman, “Mip-NeRF 360: Unbounded Anti-Aliased Neural Radiance Fields,” in Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, 2022, pp. 5470–5479.

[4] M. Tancik et al., “Nerfstudio: A Modular Framework for Neural Radiance Field Development.” arXiv, Feb. 08, 2023. doi: 10.48550/arXiv.2302.04264.

[5] K. Zhang, G. Riegler, N. Snavely, and V. Koltun, “NeRF++: Analyzing and Improving Neural Radiance Fields.” arXiv, Oct. 21, 2020. doi: 10.48550/arXiv.2010.07492.

[6] S. Fridovich-Keil, A. Yu, M. Tancik, Q. Chen, B. Recht, and A. Kanazawa, “Plenoxels: Radiance Fields Without Neural Networks,” in Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, 2022, pp. 5501–5510.

[7] A. Chen, Z. Xu, A. Geiger, J. Yu, and H. Su, “TensoRF: Tensorial Radiance Fields,” in Computer Vision – ECCV 2022, S. Avidan, G. Brostow, M. Cissé, G. M. Farinella, and T. Hassner, Eds., in Lecture Notes in Computer Science. Cham: Springer Nature Switzerland, 2022, pp. 333–350. doi: 10.1007/978-3-031-19824-3_20.

[8] A. Knapitsch, J. Park, Q.-Y. Zhou, and V. Koltun, “Tanks and temples: benchmarking large-scale scene reconstruction,” in ACM Trans. Graph., vol. 36, no. 4, p. 78:1-78:13, Jul. 2017, doi: 10.1145/3072959.3073599.

[9] B. Mildenhall, P. P. Srinivasan, M. Tancik, J. T. Barron, R. Ramamoorthi, and R. Ng, “NeRF: representing scenes as neural radiance fields for view synthesis,” in Commun. ACM, vol. 65, no. 1, pp. 99–106, Dec. 2021, doi: 10.1145/3503250.

[10] B. Foundation, “Blender - a 3D modelling and rendering package.” Stichting Blender Foundation, Amsterdam, 2018.

[11] ITU-R, “BT.500-14: Methodologies for the subjective assessment of the quality of television images,” 2019.
