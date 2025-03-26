## Project Structure
This folder contains a sample of images used and generated for the pipelines. The actual datasets can be downloaded from [TrashNet](https://www.kaggle.com/datasets/feyzazkefe/trashnet) and [RealWaste](https://www.kaggle.com/datasets/joebeachcapital/realwaste/data)

`dataset_split` : contains examples of images from the train and validation sets (RealWaste) and Testing (TrashNet) <br>
`dataset_balanced/train` : the training set used for the pipeline using Image Manipulation, by category.  <br>
`dataset_erasing_augmented/train`: the training set used for the pipeline using Image Erasing, by category.  <br>
`data/dataset_diffusion_balanced/train` : the training set used for the pipeline using Diffusion Models, by category.  <br>
`combined_dataset/train` : the training set used for combined pipeline through downsampling, by category.  <br>


