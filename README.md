# NeRF-QA: Neural Radiance Fields Quality Assessment Database

Pedro Martin, António Rodrigues, João Ascenso, Maria Paula Queluz

Instituto de Telecomunicações, Instituto Superior Técnico, University of Lisbon

Paper: https://ieeexplore.ieee.org/document/10178625

![DSCQS](https://github.com/pedrogcmartin/NeRF-QA-Database/blob/main/github%20images/DSCQS.jpg)

The Neural Radiance Fields Quality Assessment (NeRF-QA) database contains: 

+ Information about visual scenes that is used for NeRF based methods training (in the "Raw Visual Scenes" folder) with eight, real and synthetic, 360-degree camera acquition visual scenes (in the "Tanks and Temples" and "Realistic Synthetic 360" folders, respectively) and eight, real and synthetic, front-facing (FF) camera acquisition visual scenes (in the "Front-facing IST" folder) that are used to train seven NeRF based methods (nameley: DVGO, Instant-NGP, Mip-NeRF 360, Nerfacto, NeRF++, Plenoxels, and TensoRF [1,2,3,4,5,6,7]);
+ Reference videos of the visual scenes (in the "Reference Videos" folder), with durations of 10s (and of 8s for 360-degree synthetics scenes);
+ Camera paths with the pose estimation of the reference videos enabling the creation of synthesized videos with the same camera path (in the "Camera Paths" folder);
+ Synthesized videos of the same test time interval of the reference videos due to the camera paths available information (in the "Synthesized Videos" folder);
+ Results of a subjective study comparing the qualities of the reference and synthesized videos by a group of 22 participants (in the "DMOS.xlsx" file).
+ **Note:** This is an updated version of the NeRF-QA database with new material (namely, the "Front-facing IST" visual scenes dataset and a new subjective test conducted on 22 participants).

The real scenes selected from *Front-Facing IST* were:
+ *Antique* (351 training images with 960x540 pixels each)
+ *Flowers* (377 training images with 960x540 pixels each)
+ *Playground2* (291 training images with 960x540 pixels each)
+ *Statue* (228 training images with 960x540 pixels each)

The synthetics scenes selected from *Front-Facing IST* were:
+ *Classroom* (300 training images with 960x540 pixels each)
+ *Mugs* (300 training images with 960x540 pixels each)
+ *Office* (300 training images with 960x540 pixels each)
+ *Tea* (300 training images with 960x540 pixels each)

The selected videos from *Tanks and Temples* were:
+ *M60* (277 training images with 1077×546 pixels each)
+ *Playground* (275 training images with 1008×548 pixels each)
+ *Train* (258 training images with 982×546 pixels each)
+ *Truck* (226 training images with 980×546 pixels each)

For the subjective test purpose, the spatial resolutions of the real scenes were uniformized with a downsampling to 960×540 pixels, followed by a cropping to 928×522 pixels.

The scenes selected from *Realistic Synthetic 360º* were:
+ *Drums* (100 training images with 800×800 pixels each)
+ *Ficus* (100 training images with 800×800 pixels each)
+ *Lego* (100 training images with 800×800 pixels each)
+ *Ship* (100 training images with 800×800 pixels each)

The NeRF methods selected for the 360-degree real scenes were:
+ DVGO [1]
+ Mip-NeRF 360 [3]
+ Nerfacto [4]
+ NeRF++ [5] 

For the synthetic scenes, the selected 360-degree synthesis methods were:
+ DVGO [1]
+ Instant-NGP [2]
+ Plenoxels [6]
+ TensoRF [7]

The NeRF methods selected for the FF real scenes were:
+ DVGO [1]
+ Mip-NeRF 360 [3]
+ Nerfacto [4]
+ NeRF++ [5] 

For the synthetic scenes, the selected FF synthesis methods were:
+ DVGO [1]
+ Instant-NGP [2]
+ Mip-NeRF 360 [3]
+ Nerfacto [4]
+ NeRF++ [5] 
+ TensoRF [7]

The selected 360-degree datasets (namely: *Tanks and Temples* and *Realistic Synthetic 360*) have already been used in published works, enabling the validation of the herein generated synthesized videos, by comparison of the obtained objective quality metrics values (using PSNR, SSIM, and LPIPS) with the values reported on those works. Lastly, the 360-degree synthetic scenes were also synthesized for the case where a subsampling with a factor of 2 was applied to the training set, seeking synthesized video qualities covering the lowest qualities range.

The Double Stimulus Continous Quality Scale (DSCQS) was selected as an evaluation method. A total of 88 pairs of stimulus (56 synthesized synthetic videos + 32 synthesized real videos, together with the respective original videos) were assessed. After the test, the resulting scores were processed according to [11] to obtain Differential Mean Opinion Score (DMOS) values for each synthesized video. More details about the subjective assessment procedure can be found in [11].

# Citation

P. Martin, A. Rodrigues, J. Ascenso and M. P. Queluz, "NeRF-QA: Neural Radiance Fields Quality Assessment Database," 2023 15th International Conference on Quality of Multimedia Experience (QoMEX), Ghent, Belgium, 2023, pp. 107-110, doi: 10.1109/QoMEX58391.2023.10178625.

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
