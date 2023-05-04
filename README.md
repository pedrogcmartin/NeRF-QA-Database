# NeRF-QA Database

The subjective assessment of novel view synthesis with Neural Radiance Fields (NeRF) based methods was conducted using eight visual scenes taken from two popular datasets, namely Tanks and Temples [1] and Realistic Synthetic 360º [2], where the former resulted from real-world 360 degrees captures of large scenarios, and the latter was obtained with Blender [3]. The selected videos from Tanks and Temples were M60, playground, train, and truck. This dataset was used as processed in [4], where the number of training frames are equal to 277, 275, 258, and 226 frames, respectively, having spatial resolutions of 1077×546, 1008×548, 982×546, and 980×546 pixels. The scenes selected from Realistic Synthetic 360º were drums, ficus, lego, and ship, having all 100 training frames with spatial resolutions of 800×800 pixels. For the subjective test purpose, the spatial resolutions of the real scenes were uniformized with a downsampling to 960×540 pixels, followed by a cropping to 928×522 pixels. For generating the reference videos, the video duration was set to 10 s for real scenes, and to 6 s for synthetic scenes. In every case, the rendered camera poses do not coincide with the training poses. 

The NeRF methods selected for the real scenes were DVGO, Mip-NeRF 360, Nerfacto, NeRF++ [4,5,6,7]. For the synthetic scenes, the selected synthesis methods were DVGO, Instant-NGP, Plenoxels, and TensoRF [5,8,9,10]. The selected datasets have already been used in published works, enabling the validation of the herein generated synthesized videos, by comparison of the obtained objective quality metrics values (using PSNR and SSIM) with the values reported on those works. Lastly, the synthetic scenes were also synthesized for the case where a subsampling with a factor of 2 was applied to the training set, seeking synthesized video qualities covering the lowest qualities range.

The Double Stimulus Continous Quality Scale (DSCQS) was selected as an evaluation method. A total of 48 pairs of stimulus (32 synthesized synthetic videos + 16 synthesized real videos, together with the respective original videos) were assessed. After the test, the resulting scores were processed according to [11] to obtain Differential Mean Opinion Score (DMOS) values for each synthesized video. More details about the subjective assessment procedure can be found in [11].

The NQ-NeRF database repository is organized as follows: the datasets used to generate the synthesized videos are in the "datasets" folder; the reference and synthesized videos used on the subjective test are in the "Reference Videos" and "Synthesized Videos" folders; and the "DMOS.xlsx" file has the subjective test DMOS results.

# References

[1] A. Knapitsch, J. Park, Q.-Y. Zhou, and V. Koltun, “Tanks and temples: benchmarking large-scale scene reconstruction,” in ACM Trans. Graph., vol. 36, no. 4, p. 78:1-78:13, Jul. 2017, doi: 10.1145/3072959.3073599.

[2] B. Mildenhall, P. P. Srinivasan, M. Tancik, J. T. Barron, R. Ramamoorthi, and R. Ng, “NeRF: representing scenes as neural radiance fields for view synthesis,” in Commun. ACM, vol. 65, no. 1, pp. 99–106, Dec. 2021, doi: 10.1145/3503250.

[3] B. Foundation, “Blender - a 3D modelling and rendering package.” Stichting Blender Foundation, Amsterdam, 2018.

[4] K. Zhang, G. Riegler, N. Snavely, and V. Koltun, “NeRF++: Analyzing and Improving Neural Radiance Fields.” arXiv, Oct. 21, 2020. doi: 10.48550/arXiv.2010.07492.

[5] C. Sun, M. Sun, and H.-T. Chen, “Direct Voxel Grid Optimization: Super-Fast Convergence for Radiance Fields Reconstruction,” in Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, 2022, pp. 5459–5469.

[6] J. T. Barron, B. Mildenhall, D. Verbin, P. P. Srinivasan, and P. Hedman, “Mip-NeRF 360: Unbounded Anti-Aliased Neural Radiance Fields,” in Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, 2022, pp. 5470–5479.

[7] M. Tancik et al., “Nerfstudio: A Modular Framework for Neural Radiance Field Development.” arXiv, Feb. 08, 2023. doi: 10.48550/arXiv.2302.04264.

[8] T. Müller, A. Evans, C. Schied, and A. Keller, “Instant neural graphics primitives with a multiresolution hash encoding,” in ACM Trans. Graph., vol. 41, no. 4, p. 102:1-102:15, Jul. 2022, doi: 10.1145/3528223.3530127.

[9] S. Fridovich-Keil, A. Yu, M. Tancik, Q. Chen, B. Recht, and A. Kanazawa, “Plenoxels: Radiance Fields Without Neural Networks,” in Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, 2022, pp. 5501–5510.

[10] A. Chen, Z. Xu, A. Geiger, J. Yu, and H. Su, “TensoRF: Tensorial Radiance Fields,” in Computer Vision – ECCV 2022, S. Avidan, G. Brostow, M. Cissé, G. M. Farinella, and T. Hassner, Eds., in Lecture Notes in Computer Science. Cham: Springer Nature Switzerland, 2022, pp. 333–350. doi: 10.1007/978-3-031-19824-3_20.

[11] ITU-R, “BT.500-14: Methodologies for the subjective assessment of the quality of television images,” 2019.
