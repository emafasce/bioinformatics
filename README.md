# Segmentation and classification on human renal tissue

In this github folder you can find:
- The report (Bioinformatics_report.pdf)
- The presentation (available also at this link: https://www.canva.com/design/DAEyXnS4_mo/saVemvrUL28bs4x03GMadA/view?utm_content=DAEyXnS4_mo&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)
- The code

In this Readme I provide a brief explanation of the project.

## MAIN TASKS

- Segmentation of cancerous images
- Classification on the type of cancer using the predictions of the best performing segmentation network as inputs

## SEGMENTATION NETWORKS USED

- U-Net
- U-Net++
- LinkNet
- MANet

## RESULTS

![alt text](https://github.com/emafasce/bioinformatics/blob/main/visualizations/bioinformatics.jpg)

### HOW TO RUN

Notebooks for the training: they are all contained in training_nbs folder. To run them, change the path for the root_folder variable, pointing to the bioinformatics folder.
It is suggested to leave use_wandb and save_model to False, since they are used to log the results and save the models locally.

Notebooks for the visualizations: they are all contained in visualizations folder.

Notebooks for the dataset: they are all contained in dataset folder.

The Predictions folder contains the segmentation predictions of the best performing model.
