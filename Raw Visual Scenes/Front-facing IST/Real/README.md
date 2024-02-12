This directory contains a costumized dataset for front-facing camera acquisition with real and synthetic visual scenes.

Four real scenes were considered in *Front-facing IST*: *Antique*, *Flowers*, *Playground2*, and *Statue*.

Each scene folder contains:

+ The traning images (351 for *Antique*, 377 for *Flowers*, 291 for *Playground2*, and 228 for *Statue*; all with a 960x540 spatial resolution)
+ The training poses (one file per training image)
+ The intrinsics for each pose

The training images, poses, and intrinsics are used as input for the NeRF based methods training.

A Canon EOS RP full-frame camera and a steadicam stabilizer system were used for acquisition. Two small-scale scenes visual scenes were acquired: *Antique* and *Flowers*; and two large-scale scenes: *Playground2* and *Statue*.