# Effective Waste Classification through Data Augmentation

## Overview
This repository contains the implementation of our work titled "Effective Waste Classification through Data Augmentation," which explores the impact of various Data Augmentation (DA) techniques, including Image Manipulation, Image Erasing, and Diffusion Models on waste classification. We utilize DenseNet-121 to analyze performance improvements, generalization, image fidelity, and computational costs. Our study introduces a structured framework for hyperparameter tuning of DA methods and provides insights into the strategic selection of DA techniques based on their inherent trade-offs.

## Key Findings
- **Enhanced Model Performance**: Our adaptive framework significantly improves model performance through balanced augmentation approaches.
- **State-of-the-Art Techniques**: Diffusion models, which are currently state-of-the-art, substantially enhance performance and generalization, despite their higher computational cost.
- **Trade-offs in Data Augmentation**: We discuss the trade-offs between different DA techniques, particularly focusing on the balance between performance enhancement and computational expenses.
- **Generalization Across Datasets**: The study highlights the importance of considering generalization to different datasets when evaluating augmentation methods.
- **Iterative pipeline for Data Augmentation**: We present a framework of iterating through multiple cycles of generation, evaluation through quantitative metrics such as KL divergence and adjustment,  to refine the augmentation strategy leading to a more effective and adaptable dataset for downstream tasks.



## Results

### RealWaste F1-score:
| Model         | Cardboard | Glass | Metal | Paper | Plastic | Trash | Weighted Avg
|--------------|----------|-----------|--------|----------|----------|----------|----------|
|trained_realwaste_baseline_densenet |	79%|	86%|	83%|	79%|	82%|	80%|81%|
|trained_realwaste_augmentation_version_02_val_densenet|	73%|	75%|	77%|	74%|	71%|	69%| 72%|
|trained_realwaste_erasing05_models_val_densenet|	77%|	78%|	81%|	78%|	73%|	81%| 77%|
|trained_diffusion_model1_val_densenet|	74%|	85%|	79%|	73%|	71%|	66%| 75%|
|trained_combined_modell_val_densenet|	76%|	84%|	78%|	78%|	76%|	73%| 77%|
|Previous versions:|	|	|	|	|	|	| |
|trained_realwaste_erasing_version_03_val_densenet|	76%|	76%|	77%|	72%|	67%|	69%| 72%|


### Trashnet F1-score:
| Model         | Cardboard | Glass | Metal | Paper | Plastic | Trash | Weighted Avg
|--------------|----------|-----------|--------|----------|----------|----------|----------|
|trained_realwaste_baseline_densenet|	39%|	41%|	52%|	58%|	32%|	1%| 43%|
|trained_realwaste_augmentation_version_02_val_densenet|	54%|	56%|	63%|	67%|	23%|	5%| 53%|
|trained_realwaste_erasing05_models_val_densenet|	49%|	59%|	58%|	57%|	45%|	6%| 52%|
|trained_diffusion_model1_val_densenet|	69%|	65%|	71%|	75%|	56%|	9%| 66%|
|trained_combined_modell_val_densenet|	64%|	67%|	70%|	74%|	50%|	11%| 64%|
|Previous versions:|	|	|	|	|	|	| |
|trained_realwaste_erasing_version_03_val_densenet|	51%|	44%|	57%|	55%|	45%|	5%| 48%|
