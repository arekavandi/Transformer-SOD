# Transformers in Small Object Detection: A Survey and Benchmark After Four Years of Operation in Computer Vision


# Generic Applications (MS COCO)

Detection performance for small-scale objects on MS COCO image dataset (eval). DC5: Dialated C5 stage, MS: Multi-scale network, IBR: Iterative bounding box refinement, TS: Two-stage detection, DCN: Deformable convnets, TTA: Test time augmentation, BD: Pre-trained on BigDetection dataset, IN: Pre-trained on ImageNet, OB: Pre-trained on Object-365. $*$ shows the results for COCO test-dev.

| Model    | Backbone | GFLOPS/FPS | #params | $\text{mAP}^{@[0.5,0.95]}$  | Epochs | URL |
| -------- | -------- | -------- | -------- | -------- | -------- | -------- |
| Faster RCNN-DC5~(NeurIPS2015)  | ResNet50   | 320/16   |166M   | 21.4   | 37   | https://github.com/trzy/FasterRCNN |
| Faster RCNN-FPN~(NeurIPS2015) | ResNet50|180/26 | 42M| 24.2|37|https://github.com/trzy/FasterRCNN  |
|Faster RCNN-FPN~(NeurIPS2015)| ResNet101|246/20| 60M |  25.2|--|https://github.com/trzy/FasterRCNN|
| RepPoints v2-DCN-MS~(NeurIPS2020)| ResNeXt101|--/--|--|34.5* |24|https://github.com/Scalsol/RepPointsV2 |
| FCOS~(ICCV2019)| ResNet50| 177/17|--|26.2|36|https://github.com/tianzhi0549/FCOS|
| CBNet V2-DCN~(TIP2022)|Res2Net101 |--/--|107M|35.7*|20|https://github.com/VDIGPKU/CBNetV2|
| CBNet V2-DCN(Cascade RCNN)~(TIP2022)| Res2Net101|--/--|146M|37.4*|32|https://github.com/VDIGPKU/CBNetV2|
| DETR~(ECCV2020)| ResNet50|86/28 | 41M | 20.5|500|https://github.com/facebookresearch/detr|

# Citations
If you found this page helpful, please cite the following survey papers:

@article{rekavandi2022guide,
  title={A Guide to Image and Video based Small Object Detection using Deep Learning: Case Study of Maritime Surveillance},
  author={Rekavandi, Aref Miri and Xu, Lian and Boussaid, Farid and Seghouane, Abd-Krim and Hoefs, Stephen and Bennamoun, Mohammed},
  journal={arXiv preprint arXiv:2207.12926},
  year={2022}
}
