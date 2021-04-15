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


When running on GPUs, from JupyterHub:
Open a new launcher (File > New Launcher in the menu bar), select the "Terminal" option, execute the nvidia-smi command there, and verify it provides the same output. Notice that there is a "GPU-Util" column, which measures the GPU's utilization. It tells you what fraction of the last second the GPU was in use. We can thus easily monitor GPU activity by regularly checking this output. One way to do that is using the Linux utility watch: watch -n 5 nvidia-smi will set up a loop that refreshes the nvidia-smi output every 5 seconds. Make sure you run that in the separate terminal window, not here in the notebook, because the notebook can only run one process at a time. You can type Ctrl+C in the terminal to end the loop later.
