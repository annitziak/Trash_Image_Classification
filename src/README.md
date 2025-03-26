## Project Structure
- **analysis_data_augmentation**: Analyzes and compares the performance impact of different data augmentation techniques using plots and metrics.
- **data_creation**: Handles the generation and organization of datasets, including directory setup and preprocessing steps.
- **diffusion_model**: Implements and applies diffusion models to generate augmented images from noise.
- **image_erasing**: Applies various image erasing techniques (e.g., Hide and Seek, CoarseDropout) to create augmented datasets.
- **Image_manipulation**: Applies image manipulation-based augmentations such as color shifting or geometric transformations.
- **model_test**: Loads trained models and evaluates them on test data, outputting metrics like accuracy and confusion matrices.
- **model_training**: Full training pipeline for DenseNet-121 including data loading, training loop, validation, and performance logging.
