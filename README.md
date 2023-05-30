# Transformers in Small Object Detection: A Survey and Benchmark After Four Years of Operation in Computer Vision


# Generic Applications (MS COCO)

Detection performance for small-scale objects on MS COCO image dataset (eval). DC5: Dialated C5 stage, MS: Multi-scale network, IBR: Iterative bounding box refinement, TS: Two-stage detection, DCN: Deformable convnets, TTA: Test time augmentation, BD: Pre-trained on BigDetection dataset, IN: Pre-trained on ImageNet, OB: Pre-trained on Object-365. $*$ shows the results for COCO test-dev.

| Model    | Backbone | GFLOPS/FPS | $\#$params | $\text{mAP}^{@[0.5,0.95]}$  | Epochs | URL |
| -------- | -------- | -------- | -------- | -------- | -------- | -------- |
| Faster RCNN-DC5~(NeurIPS2015)  | ResNet50   | 320/16   |166M   | 21.4   | 37   | https://github.com/trzy/FasterRCNN |
| Faster RCNN-FPN~(NeurIPS2015) | ResNet50|180/26 | 42M| 24.2|37|https://github.com/trzy/FasterRCNN  |
|Faster RCNN-FPN~(NeurIPS2015)| ResNet101|246/20| 60M |  25.2|--|https://github.com/trzy/FasterRCNN|
