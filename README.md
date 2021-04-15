# Machine Learning Object Detection

This repo is setup up to provide notebooks that work with either Kubeflow or OpenDataHub deployments.

## Current Notebooks:
|notebook|description|
|-|-|
|ship-model-build-1of2.ipynb|performs setup notebook to save model|
|ship-model-deploy-2of2.ipynb|performs import model to inference on new data|

# Folders
|||
|-|-|
|notebooks|there are variations between the tools kubeflow and opendatahub install causing notebooks to fail if not set|
|notebooks > kubeflow|if you installed kubeflow, run these|
|notebooks > opendatahub|if you installed opendatahub, run these|
|dataset|a training dataset with 4000 80x80x3 images from Kaggle with ship and no-ship labelled|
|images|imagery that can be replace .png file paths in the notebook for demonstration purposes|
|models|to be uploaded. Currently, saved in the namespace hosting the notebook|

> Notebooks are CPU capable. GPUS notebooks will be specified in the name.
