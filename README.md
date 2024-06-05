# A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells


<H3>Dataset information</H3>
The dataset consists of 481 visual fields, of which 312 are randomly sampled from more than 20K whole slide images at different magnifications, from multiple data sources. In total the dataset contains 205,343 labeled nuclei, each with an instance segmentation mask.

The ground truth annotation samples are shown in the figure below:
![annotations](https://github.com/srinivas21109/A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells/assets/119849011/fa713608-3a61-4c63-a6aa-25d659778ea8)

Annotations

Each instance of the 5 cell classes are annotated separately (Red: Neoplastic; Green: Inflammatory; Dark Blue: Connective; Yellow: Dead; Orange: Epithelial)

The MaskRCNN instance segmentation model was developed using Facebook AI reseach's (FAIR) Detectron 2 framework.
