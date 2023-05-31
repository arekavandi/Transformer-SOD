# Transformers in Small Object Detection: A Survey and Benchmark After Four Years of Operation in Computer Vision
For adding your results to the tables below, please send us an email including the values for each column and a copy of the paper showing your results.
Email: aref.mirirekavandi@gmail.com

# Generic Applications (MS COCO) (Last Update: 31/05/2023)

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
|**Best Results**|NA|DETR&FP-DETR|Group DETR v2|DINO|NA|

# Citations
If you found this page helpful, please cite the following survey papers:

@article{rekavandi2022guide,
  title={A Guide to Image and Video based Small Object Detection using Deep Learning: Case Study of Maritime Surveillance},
  author={Rekavandi, Aref Miri and Xu, Lian and Boussaid, Farid and Seghouane, Abd-Krim and Hoefs, Stephen and Bennamoun, Mohammed},
  journal={arXiv preprint arXiv:2207.12926},
  year={2022}
}
