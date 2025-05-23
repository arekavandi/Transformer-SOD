[![arXiv](https://img.shields.io/badge/arXiv-2309.04902-b31b1b.svg)](https://arxiv.org/abs/2309.04902)

# Transformers in Small Object Detection: A Benchmark and Survey of State-of-the-Art
**For adding your transformer-based object detector results into the tables below, please send us an email including the values for each column and a copy of the paper showing your results.**

Email: aref.mirirekavandi@gmail.com
Email: shima.rashidi7@gmail.com

## Taxonomy
Taxonomy of small object detection using transformers and popular object detection methods assigned to each category.
![image](https://github.com/arekavandi/Transformer-SOD/assets/101369948/05becaf3-1931-4c1e-a8eb-b9d8b5f06514)

## Datasets
![image](https://github.com/arekavandi/Transformer-SOD/assets/101369948/39e34dc3-079c-4057-a9e7-2a4e56d83900)


# Generic Applications (MS COCO) (Last Update: 15/06/2023)

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
|DETR-DC5~(ECCV2020)| ResNet50|187/12| 41M|22.5|500|https://github.com/facebookresearch/detr|
|DETR~(ECCV2020)| ResNet101|52/20| 60M|21.9|--|https://github.com/facebookresearch/detr|
|DETR-DC5~(ECCV2020)|ResNet101|253/10 | 60M| 23.7|--|https://github.com/facebookresearch/detr|
|ViT-FRCNN~(arXiv2020)|--|--/-- | --| 17.8|--|--|
|RelationNet++~(NeurIPS2020)|ResNeXt101|--/-- | --| 32.8*|--|https://github.com/microsoft/RelationNet2|
|RelationNet++-MS~(NeurIPS2020)|ResNeXt101|--/-- | --| 35.8*|--|https://github.com/microsoft/RelationNet2|
|Deformable DETR~(ICLR2021)| ResNet50| 173/19| 40M|26.4|50| https://github.com/fundamentalvision/Deformable-DETR|
|Deformable DETR-IBR~(ICLR2021)| ResNet50| 173/19| 40M| 26.8| 50|https://github.com/fundamentalvision/Deformable-DETR|
|Deformable DETR-TS~(ICLR2021)| ResNet50|173/19 |40M |28.8| 50|https://github.com/fundamentalvision/Deformable-DETR|
|Deformable DETR-TS-IBR-DCN~(ICLR2021)|ResNeXt101|--/-- |--  |34.4*| --|https://github.com/fundamentalvision/Deformable-DETR|
|Dynamic DETR~(ICCV2021)|ResNet50|--/-- |-- |28.6*| --|--|
|Dynamic DETR-DCN~(ICCV2021)|ResNeXt101|--/-- |-- |30.3*| --|--|
|TSP-FCOS~(ICCV2021)|ResNet101|255/12|--|27.7|36|https://github.com/Edward-Sun/TSP-Detection|
|TSP-RCNN~(ICCV2021)|ResNet101|254/9|--|29.9|96|https://github.com/Edward-Sun/TSP-Detection|
|Mask R-CNN~(ICCV2021)|Conformer-S/16| 457/--| 56.9M|28.7|12|https://github.com/pengzhiliang/Conformer|
|Conditional DETR-DC5~(ICCV2021)|ResNet101 |262/--| 63M| 27.2|108 | https://github.com/Atten4Vis/ConditionalDETR|
|SOF-DETR~(2022JVCIR) | ResNet50 | --/--| --| 21.7| --| https://github.com/shikha-gist/SOF-DETR/|
|DETR++~(arXiv2022)| ResNet50 | --/--|-- | 22.1|-- |--|
|TOLO-MS~(NCA2022) | --|--/57|--|24.1|--|--|
|Anchor DETR-DC5~(AAAI2022) |ResNet101|--/--|--|25.8|50| https://github.com/megvii-research/AnchorDETR|
|DESTR-DC5~(CVPR2022)| ResNet101| 299/--|88M|28.2|50|--|
|Conditional DETR v2-DC5~(arXiv2022)|ResNet101 |228/--| 65M| 26.3|50 | --|
|Conditional DETR v2~(arXiv2022)|Hourglass48 |521/--| 90M| 32.1|50|-- |
|FP-DETR-IN~(ICLR2022) | --| --/--|36M |26.5 | 50|https://github.com/encounter1997/FP-DETR|
|DAB-DETR-DC5~(arXiv2022)| ResNet101| 296/--| 63M| 28.1| 50| https://github.com/IDEA-Research/DAB-DETR|
|Ghostformer-MS~(Sensors2022)| GhostNet| --/--| --| 29.2| 100|--|
|CF-DETR-DCN-TTA~(AAAI2022)|ResNeXt101 |--/-- | --|35.1*|--|--|
|CBNet V2-TTA~(CVPR2022)|Swin Transformer-base |--/--|--|41.7|--|https://github.com/amazon-science/bigdetection|
|CBNet V2-TTA-BD~(CVPR2022)|Swin Transformer-base |--/--|--|42.2|--|https://github.com/amazon-science/bigdetection|
|DETA~(arXiv2022)|ResNet50| --/13|48M| 34.3|24|https://github.com/jozhang97/DETA|
|DINO~(arXiv2022)| ResNet50|860/10| 47M| 32.3|12| https://github.com/IDEA-Research/DINO|
|CO-DINO Deformable DETR-MS-IN~(arXiv2022)| Swin Transformer-large|--/--|--| 43.7|36|https://github.com/Sense-X/Co-DETR|
|HYNETER~(ICASSP2023)| Hyneter-Max| --/--|247M|29.8*|--|-- |
|DeoT~(JRTIP2023) | ResNet101 | 217/14 | 58M| 31.4| 34|--|
|ConformerDet-MS~(TPAMI2023)| Conformer-B | --/-- | 147M|35.3 | 36 | https://github.com/pengzhiliang/Conformer|
|YOLOS~(NeurIPS2021)|DeiT-base|--/3.9|100M|19.5|150|https://github.com/hustvl/YOLOS|
|DETR(ViT)~(arXiv2021)|Swin Transformer-base|--/9.7|100M|18.3|50|https://github.com/naver-ai/vidt|
|Deformable DETR(ViT)~(arXiv2021)|Swin Transformer-base|--/4.8|100M|34.5|50|https://github.com/naver-ai/vidt|
|ViDT~(arXiv2022)|Swin Transformer-base|--/9|100M|30.6|50|https://github.com/naver-ai/vidt/tree/main|
|DFFT~(ECCV2022) | DOT-medium| 67/--| --| 25.5| 36| https://github.com/PeixianChen/DFFT|
|CenterNet++-MS~(arXiv2022) | Swin Transformer-large |--/--|--|38.7*|--|https://github.com/Duankaiwen/PyCenterNet|
|DETA-OB~(arXiv2022)|Swin Transformer-large| --/4.2|--| 46.1*|24|https://github.com/jozhang97/DETA|
|Group DETR v2-MS-IN-OB~(arXiv2022) | ViT-Huge| --/--|629M| 48.4*|--|-- |
|**Best Results**|NA|DETR/TOLO|FP-DETR|Group DETR v2|DINO|NA|

# Small Object Detection in Aerial Images (DOTA) (Last Update: 15/06/2023)

Detection performance for objects on DOTA image dataset. MS: Multi-scale network, FT: Fine-tuned, FPN: Feature pyramid network, IN: Pre-trained on ImageNet.

| Model    | Backbone | FPS | #params | mAP  | Epochs | URL |
| -------- | -------- | -------- | -------- | -------- | -------- | -------- |
| Rotated Faster RCNN-MS~(NeurIPS2015)  | ResNet101   | --   |64M   | 67.71   | 50   | https://github.com/open-mmlab/mmrotate/tree/main/configs/rotated_faster_rcnn |
|SSD~(ECCV2016) |-- |-- | --|56.1| --|https://github.com/pierluigiferrari/ssd_keras|
|RetinaNet-MS~(ICCV2017)| ResNet101| --|59M|66.53|50|https://github.com/DetectionTeamUCAS/RetinaNet_Tensorflow|
|ROI-Transformer-MS-IN~(CVPR2019) | ResNet50|-- | --|80.06|12 | https://github.com/open-mmlab/mmrotate/blob/main/configs/roi_trans/README.md|
|Yolov5~(2020)|-- |95| --|64.5| --| https://github.com/ultralytics/yolov5|
|ReDet-MS-FPN~(CVPR2021)| ResNet50| --|--|80.1|--|https://github.com/csuhan/ReDet|
|O2DETR-MS~(arXiv2021)| ResNet101|-- | 63M|70.02|50|--|
|O2DETR-MS-FT~(arXiv2021)| ResNet101|-- | --| 76.23|62|--|
|O2DETR-MS-FPN-FT~(arXiv2021)| ResNet50|-- | --| 79.66|--|--|
|SPH-Yolov5~(RS2022) | Swin Transformer-base |51 |-- | 71.6| 150|--|
|AO2-DETR-MS~(TCSVT2022)| ResNet50| --| --| 79.22|--|https://github.com/Ixiaohuihuihui/AO2-DETR|
|MDCT~(RS2023)|-- |-- | --|75.7| --| --|
|ReDet-MS-IN~(arXiv2023)| ViTDet, ViT-B|--|--|80.89|12|https://github.com/csuhan/ReDet|
|**Best Results**|NA|Yolov5|RetinaNet|ReDet-MS-IN|ReDet-MS-IN|NA|

# Small Object Detection in Medical Images (DeepLesion) (Last Update: 15/06/2023)

Detection performance for DeepLesion CT image dataset.

| Model    | Accuracy |$\text{mAP}^{0.5}$ | 
| -------- | -------- | --------  |
|Faster RCNN~(NeurIPS2015)| 83.3 |83.3|
|Yolov5 |85.2 |88.2|
|DETR~(ECCV2020)|86.7 |87.8|
|Swin Transformer| 82.9|81.2|
|MS Transformer~(CIN2022)|90.3|89.6|
|**Best Results**|MS Transformer|MS Transformer|

# Small Object Detection in Active Milli-Meter Wave Images (AMWW) (Last Update: 15/06/2023)

Detection performance for AMWW image dataset. 

| Model    | Backbone| $\text{mAP}^{0.5}$ | $\text{mAP}^{@[0.5,0.95]}$|
| -------- | -------- | --------  |--------|
|Faster RCNN~(NeurIPS2015)|ResNet50 |70.7| 26.83|
|Cascade RCNN~(CVPR2018)|ResNet50 | 74.7 | 27.8|
|TridentNet~(ICCV2019) |ResNet50|77.3|29.2|
|Dynamic RCNN~(ECCV2020) | ResNet50| 76.3| 27.6|
|Yolov5 |ResNet50 |76.67| 28.48|
|MATR~(TCSVT2022) | ResNet50| 82.16 | 33.42|
|**Best Results**|NA|MATR|MATR|


# Small Object Detection in Underwater Images (URPC2018) (Last Update: 15/06/2023)

Detection performance for URPC2018 dataset. 

| Model    | #params | $\text{mAP}^{@[0.5,0.95]}$| $\text{mAP}^{0.5}$|
| -------- | -------- | --------  |--------|
|Faster RCNN~(NeurIPS2015)|33.6M| 16.4|--|
|Cascade RCNN~(CVPR2018)| 68.9M| 16|--|
|Dynamic RCNN~(ECCV2020) |41.5M| 13.3|--|
|Yolov3 | 61.5M| 19.4|--|
|RoIMix~(ICASSP2020) | --|-- |74.92|
|HTDet~(RS2023) |7.7M|22.8|--|
|**Best Results**|HTDet|HTDet|RoIMix|

# Small Object Detection in Videos (ImageNet VID) (Last Update: 15/06/2023)

Detection performance for ImageNet VID dataset for small objects. PT: Pre-trained on MS COCO.

| Model    | Backbone |$\text{mAP}^{@[0.5,0.95]}$| 
| -------- | -------- | --------  |
|Faster RCNN~(NeurIPS2015)+SELSA| ResNet50| 8.5|
|Deformable-DETR-PT |ResNet50|10.5|
|Deformable-DETR+TransVOD-PT|ResNet50|11|
|DAB-DETR+FAQ-PT|ResNet50|12|
|Deformable-DETR+FAQ-PT|ResNet50|13.2|
|**Best Results**|NA|Deformable DET+FAQ|

## Visual Results
Detection results on a sample image when zoomed in. First row from the left: Input image, SSD, Faster RCNN, DETR. Second row from the left: ViDT, DETA-OB, DINO, CBNetv2.
![image](https://github.com/arekavandi/Transformer-SOD/assets/101369948/b9151625-a327-4131-94f7-eb654407c0da)



# Citations
If you found this page helpful, please cite the following survey paper:

```
@article{rekavandi2023transformers,
  title={Transformers in Small Object Detection: A Benchmark and Survey of State-of-the-Art},
  author={Rekavandi Miri, Aref and Rashidi, Shima and Boussaid, Farid and Hoefs, Stephen and Akbas, Emre and Bennamoun, Mohammed},
  journal={arXiv preprint arXiv:2309.04902},
  year={2023}
}

```

