# SLEAP sample datasets

Sample datasets for using with [SLEAP](https://github.com/talmolab/sleap).

## Drosophila melanogaster courtship example

Download the dataset: [drosophila-melanogaster-courtship.zip](https://github.com/talmolab/sleap-datasets/releases/download/dm-courtship-v1/drosophila-melanogaster-courtship.zip).

This dataset has 100 labeled frames (2 flies/frame) and 1101 frames in the movie.

![](drosophila-melanogaster-courtship/example.jpg)

### Baseline training and inference times

GPU: [NVIDIA GeForce GTX 2080](https://www.nvidia.com/en-us/geforce/graphics-cards/rtx-2080/)

Training top-down models for 20 epochs with default baseline profiles:

- 7 minutes to train centroid model
- 3.1 minutes to train centered instance model

Inference:

- 1 minute for inference on all 1101 frames of sample dataset video (no tracking)
- 7.2 minutes for inference and tracking (simple tracker) on 10,000 frames from original video (~23 fps)

![](https://raw.githubusercontent.com/talmolab/sleap-datasets/master/previews/courtship-dataset-clip-small.gif)

(or watch the higher-resolution [tracked clip](http://www.youtube.com/watch?v=hYNN7GTjUFo))

## Downloading all datasets

You can download the entire repository by running

`git clone https://github.com/talmolab/sleap-datasets.git`

Unfortunately the "Download ZIP" link on this repository won't work because we store videos using [Git Large File Storage](https://git-lfs.github.com).
