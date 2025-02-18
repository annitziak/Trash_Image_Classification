# mlp_assignment

Update `proposal.md`

https://www.notion.so/Machine-Learning-Practical-1889f99a47b6801c8a6cc4bfd2c73cac?pvs=4  <br>
`new template` : https://www.overleaf.com/8581932666vtycckjvtkgy#5487f5 <br>

`old`:https://www.overleaf.com/9113767633wtpbydgfbdxr#6c98a0

## Results

### RealWaste F1-score:
| Model         | Cardboard | Glass | Metal | Paper | Plastic | Trash | 
|--------------|----------|-----------|--------|----------|----------|----------|
|trained_realwaste_baseline_densenet      | 84%    | 86%     | 85%  | 87%    | 82%  | 83%    |
|trained_realwaste_augmentation_version_02_val_densenet      | 79%    | 79%     | 82%  | 82%    | 77% | 76% |
| trained_trashnet_densenet|	38%|	30%|	60%|	54%|	59%|	6%|


### Trashnet F1-score:
| Model         | Cardboard | Glass | Metal | Paper | Plastic | Trash | 
|--------------|----------|-----------|--------|----------|----------|----------|
|trained_realwaste_baseline_densenet      | 39%    | 41%     | 52%  | 58%    | 32% | 1% |
|trained_realwaste_augmentation_version_02_val_densenet      | 54%    | 56%     | 63%  | 67%    | 23% | 5% |
| trained_trashnet_densenet|	41%|	34%|	59%|	51%|	52%|	9%|
