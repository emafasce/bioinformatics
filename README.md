# Segmentation and classification on human renal tissue

This is the Bioinformatics project "Segmentation on human renal tissue". In this github folder you can find the Latex document, the presentation and all the code I wrote.
In this Readme I provided a very high level view of the contents of this project and a brief explanation on how to run the code.

### MAIN TASKS

- Segmentation of cancerous images
- Classification on the type of cancer using the predictions of the best performing segmentation network as inputs


### EXPLORED TOPICS

Segmentation

- Which model and backbone performs better on the segmentation task?
- Which transformations are more useful?
- Which loss function works better?

Classification

- Are segmentation predictions useful to classify the two types of cancer?


### NOTEBOOKS DESCRIPTION

Notebooks for the training: they are all contained in training_nbs folder. To run them, make a Wandb account (1) and change the paths.
Notebooks for the visualizations: they are all contained in visualizations folder.
Notebooks for the dataset: they are all contained in dataset folder


### APPENDIX

(1): In this project I used Wandb to log the results.
