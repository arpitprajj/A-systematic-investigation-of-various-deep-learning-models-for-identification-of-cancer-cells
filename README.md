# A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells


<H2>[Project_report.pdf](https://github.com/user-attachments/files/15580615/Project_report.pdf)</H2>


<H3>Proposed Workflow</H3> 
<BR></BR>
Our proposed workflow includes five main stages: Data Preprocessing, Model Selection and Training, Model Evaluation and Comparison, Model Selection and Fine-Tuning, and Final Evaluation and Results. The diagram below describes the workflow stepwise.

![Picture1](https://github.com/srinivas21109/A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells/assets/119849011/270770c6-d2c1-4b76-a82a-f1ce1294e8a7)

<br>

<H3>Dataset information</H3>
The dataset consists of 481 visual fields, of which 312 are randomly sampled from more than 20K whole slide images at different magnifications, from multiple data sources. In total the dataset contains 205,343 labeled nuclei, each with an instance segmentation mask.

The ground truth annotation samples are shown in the figure below:

![Picture2](https://github.com/srinivas21109/A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells/assets/119849011/fa713608-3a61-4c63-a6aa-25d659778ea8)

<H3>Data Preprocessing</H3>

The Pannuke data downloaded is in the form of numpy file. It contains images.npy and types.npy. After that we loaded the data using np.load(). Next we reduced the size using astype(np.int16). Then we removed Images without cells following by index splitting. In last we organized all the image files. Using pycococreator tool, we are making coco.json file for our image files with categories neoplastic, inflammatory, softtissue, dead, epithelial.The coco.json file will be used for annotations as well as labelling.Further we apply image preprocessing techniques.

The Steps involved in data preprocessing are shown in figure below:
![Picture2](https://github.com/srinivas21109/A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells/assets/119849011/a272fe9d-67b3-406c-b79c-5531a579a393)

<br>

<H3>Architecture of Unet with EfficientnetB7 Encoder</H3>

![Picture3](https://github.com/srinivas21109/A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells/assets/119849011/8b01899e-cb08-4e07-9351-ecc0b0307680)

<H2 align:center >Sematic segmentation of six classes using u-net with efficientnetb7</H2></p>

![Picture6](https://github.com/srinivas21109/A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells/assets/119849011/66c982fc-cfc7-4122-9e5b-711afaa3eaf5)

<br>

<H3>Architecture of Detectron2</H3>

![Picture4](https://github.com/srinivas21109/A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells/assets/119849011/441cf0a7-34b0-41e7-bb44-53ed4563888d)

<br>
<H3>Architecture of YOLOV8</H3>

![Picture5](https://github.com/srinivas21109/A-systematic-investigation-of-various-deep-learning-models-for-identification-of-cancer-cells/assets/119849011/d6a992d5-7fe5-4b4e-bb2e-5fc32899267f)




