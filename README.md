# Final Year Project - Investigating the Impact of Inset Emojis on Images in News Articles

## Author:
Isaac Muscat

## Supervisor:
Dr Dylan Seychell


This project consists of a dataset of emojis inset onto normal background images. The dataset for classification can be found in **Classification_Dataset**, which consists of a **Train**, **Val** and **Test** folder, each of which comprises inset and non-inset images. The object detection folder, **Object_Detection_Dataset**, has a similar composition, however three annotation types are created: **CSV**, **VOC XML** and **YOLO**. Each of these folder consist of the training, validation and testing subfolders, in which are the image subfolders as well as the annotations.

The datasets to create this dataset were a subset of the **COCO** dataset, whose installing notebook is provided within this project, as well as the Facebook Emojis dataset, which are also available within these project folders in the **FacebookEmojis** folder. 

The Python Notebook **Emoji_Inset_Creator.ipynb** was used to generate the dataset by utilising the two pre-existing datasets, however the notebook was made to easily have the datasets required altered by simply changing the file location from which to retrieve the dataset. Furthermore, to clear the current existing dataset to create a new one, the **clearFolder.ipynb** notebook can be used. For evaluation purposes, the **centrebias.ipynb** notebook provides a graph to depict the regions at which a high focus of emoji centroids can be found, on which the current dataset provides an even distribution.

For object detection training and evaluating, the **YOLOv8** subfolder contains the **Emoji_Image_Object_Detection_YOLOv8.ipynb** notebook, used to for everything related to the YOLOv8 model, including its training, validation and testing segments. This model also utilises the **data.yaml** file which provides information on the different set locations and labels to be used in training for the YOLOv8 model. Moreover, the **runs** folder saves information of the testing performed on the model, including graphs generated. For RetinaNet training and evaluating, the **Retinanet** subfolder contains the **Emoji_Image_Object_Detection_Retinanet.ipynb** notebook which is responsible for training and testing its respective model. The **Retinanet** subfolder consists of other files and folders required to run and evaluate the Retinanet model. 

<p align="center">
  <img src="./University-of-Malta.png" alt="University Logo" width="200"/>
</p>
