# Segmentation and classification on human renal tissue

## MAIN TASKS

In this project several neural architectures for segmentation are implemented and evaluated on a dataset composed of 200 images of cancerous cells depicting two types of cancer,  Clear cell renal cell carcinoma and Papillary renal cell carcinoma.
The best performing model is then used to build another classification dataset composed of its predictions as input images and the type of cancer as label: a ResNet that uses the predictions as input images predicts the type of cancer surprisingly well, further validating the segmentation task.

## SEGMENTATION NETWORKS USED

- U-Net
- U-Net++
- LinkNet
- MANet

## RESULTS

- The elastic + affine transformations improve the results
- The ResNest backbone works best
- Using bigger input images helps the performance
- The best runs of each model have similar performances, probably due to the models similarity, as shown by the next table.



![alt text](https://github.com/emafasce/bioinformatics/blob/main/visualizations/results.png)


These are two predictions from the best performing model, the U-Net++, on the test set.
On the visualization on the right, a TP is indicated by green, FP by blue, TN by white, FN by red.


![alt text](https://github.com/emafasce/bioinformatics/blob/main/visualizations/bioinformatics.jpg)

This model achieves 65.10% IOU on the test set. The predictions of this model are used to build another classification dataset, with the type of cancer as label.  A ResNet50 easily reaches 100% accuracy on the test set of this last dataset.


## REPO CONTENT

In this repo you can find:
- The report (Bioinformatics_report.pdf)
- The presentation (available also at this link: https://www.canva.com/design/DAEyXnS4_mo/saVemvrUL28bs4x03GMadA/view?utm_content=DAEyXnS4_mo&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)
- The code

### HOW TO RUN

Notebooks for the training: they are all contained in training_nbs folder. To run them, change the path for the root_folder variable, pointing to the bioinformatics folder.
It is suggested to leave use_wandb and save_model to False, since they are used to log the results and save the models locally.

Notebooks for the visualizations: they are all contained in visualizations folder.

Notebooks for the dataset: they are all contained in dataset folder.

The Predictions folder contains the segmentation predictions of the best performing model.
