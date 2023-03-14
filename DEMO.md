Basic installations (tested on Ubuntu 22.04 with GPU 3050 RTX)


conda create -n dekr_env python=3.6

This repo needs installation pf pycocotools and crowdpose. Clone the repositories and install as per installation instructions in repo

Download the pretrained models (link: https://mailustceducn-my.sharepoint.com/:f:/g/personal/aa397601_mail_ustc_edu_cn/EmoNwNpq4L1FgUsC9KbWezABSotd3BGOlcWCdkBi91l50g?e=HWuluh) and extract the model.zip in DEKR/ pofilder

To run the inference on a video, use following command

```
conda activate dekr_env
python tools/inference_demo.py --cfg experiments/coco/inference_demo_coco.yaml --videoFile metro-2.avi --outputDir output --visthre 0.3 TEST.MODEL_FILE model/pose_coco/pose_dekr_hrnetw32_coco.pth

```
