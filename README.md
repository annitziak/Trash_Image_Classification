# mlp_assignment

Update `proposal.md`

https://www.notion.so/Machine-Learning-Practical-1889f99a47b6801c8a6cc4bfd2c73cac?pvs=4  <br>
`new template` : https://www.overleaf.com/8581932666vtycckjvtkgy#5487f5 <br>

`old`:https://www.overleaf.com/9113767633wtpbydgfbdxr#6c98a0

## Results

### RealWaste F1-score:
| Model         | Cardboard | Glass | Metal | Paper | Plastic | Trash | Total Accuracy
|--------------|----------|-----------|--------|----------|----------|----------|----------|
|trained_realwaste_baseline_densenet |	79%|	86%|	83%|	79%|	82%|	80%|82%|
|trained_realwaste_augmentation_version_02_val_densenet|	73%|	75%|	77%|	74%|	71%|	69%| 73%|
|trained_realwaste_erasing05_models_val_densenet|	77%|	78%|	81%|	78%|	73%|	81%| 78%|
|Previous versions:|	|	|	|	|	|	| |
|trained_realwaste_erasing_version_03_val_densenet|	76%|	76%|	77%|	72%|	67%|	69%| 73%|


### Trashnet F1-score:
| Model         | Cardboard | Glass | Metal | Paper | Plastic | Trash | Total Accuracy
|--------------|----------|-----------|--------|----------|----------|----------|----------|
|trained_realwaste_baseline_densenet|	39%|	41%|	52%|	58%|	32%|	1%| 44%|
|trained_realwaste_augmentation_version_02_val_densenet|	54%|	56%|	63%|	67%|	23%|	5%| 54%|
|trained_realwaste_erasing05_models_val_densenet|	49%|	59%|	58%|	57%|	45%|	6%| 53%|
|Previous versions:|	|	|	|	|	|	| |
|trained_realwaste_erasing_version_03_val_densenet|	51%|	44%|	57%|	55%|	45%|	5%| 49%|
