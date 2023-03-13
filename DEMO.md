Basic installations (tested on Ubuntu 22.04 with GPU 3050 RTX)


conda create -n dekr_env python=3.6

This repo needs installation pf pycocotools and crowdpose. Clone the repositories and install as per installation instructions in repo

Download the pretrained models and extract the model.zip

To run the inference on a video, use following command

```
conda activate dekr_env
python tools/inference_demo.py --cfg tools/inference_demo_coco.yaml --videoFile tools/metro.avi 

```
