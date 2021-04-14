# Machine Learning Object Detection

This repo is setup up to provide notebooks that work with either Kubeflow or OpenDataHub deployments.

Current Notebooks:
1. ship-model-object-all-in-1.ipynb (all in 1 notebook from setup to inference)
1. ship-model-build-1of2.ipynb (breaksup all-in-1, setup to save)
1. ship-model-deploy-2of2.ipynb (breasup all-in-1, deploy to inference)

# Folders
1. notebooks
   1. kubeflow = if you installed kubeflow, run these
   1. opendatahub = if you installed opendatahub, run these
      1. NVIDIA GPU Operator = if you configured the kfdef and imagestreams for GPUs, run these
1. dataset = a training dataset with 4000 80x80x3 images from Kaggle with ship and no-ship labelled
1. images = imagery that can be replace .png file paths in the notebook for demonstration purposes
1. models = to be uploaded. Currently, saved in the namespace hosting the notebook.
