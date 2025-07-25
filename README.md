# mri_mp2rage_segmentation

## description
A model for segmenting MP2RAGE MRI images and removing background noise

The model comes with a trainer that can be used to train it using data, preferably from the MPI-LEMON dataset(slices of size [256, 240]):
https://fcon_1000.projects.nitrc.org/indi/retro/MPI_LEMON/downloads/download_MRI.html

Pre-trained parameters are also included and can be directly used to remove the background from t1map images without additional training

## requirements
This model was built and tested in Python 3.11.13, be careful when using older versions of Python
The training should take ~1 minute for 1 epoch using a GPU with ~40GB of memory
Make sure to verify the file names and the image sizes before use
Note that the validation images were resized to [256, 240] when generating the mask to save memory
