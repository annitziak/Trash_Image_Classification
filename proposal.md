### Proposal Annie

**Problem Statement:**
Waste classification has achieved high performance with some architectures, but dataset variation remains a significant challenge (most papers say this). 
We hypothesize that advanced data augmentation techniques will improve model performance and generalization.

**Methods:**
1. **Traditional Augmentation:** Standard techniques like flipping, cropping, rotation, scaling, and color jittering to serve as a baseline. -> very easy to impleement
2. **Text-to-Image Models:** Leverage diffusion models (e.g., Stable Diffusion - very easy `StableDiffusionPipeline.from_pretrained(model_id)` and can finetune on the Trashnet dataset) and LLM-guided text-to-image generation to create diverse, class-specific synthetic data. -> we can play with propmts NLP 
4. **GAN-Based Augmentation:** Optional (some papers showed its not promising)
**Models:**
1. **Convolutional Neural Networks (CNNs):** Including advanced architectures like ResNets.
2. **Vision Transformers (ViTs):** Assess performance with transformer-based models. -not a lot of research for trash

**Objective:**
Evaluate the impact of various augmentation methods on classification accuracy, and generalization in waste classification.


### Proposal Vasilis

**Problem Statement:**
It is very costly and unhealthy to label the images, which is why the several datasets that exist have a limited number of data. The following paper (from 2024) tried semi-supervised learning and improved the accuracy by 3.5%.
We hypothesize that different semi-supervised techniques that exist can further improve the accuracy as long as improving the adaptive weighted loss function.

**Datasets:** (Qi, J., Nguyen, M., & Yan, W. Q. (2024). NUNI-Waste: novel semi-supervised semantic segmentation waste classification with non-uniform data augmentation. Multimedia Tools and Applications, 1-19.)
1. **Zerowaste:** Zerowaste-f, Zerowaste-s, and Zerowaste-w. We mainly take use of the Zerowaste-s dataset, which is available for semi-supervised tasks and contains 6,212 unlabeled images, (Cardboard, Soft plastic, Rigid plastic, and Metal)

**Datasets:** (Majchrowska, Sylwia, et al. "Deep learning-based waste detection in natural and urban environments." Waste Management 138 (2022): 274-284.)
1. **Open Litter Map:** 100k images, labeled, (information such as type of presented litter, coordinates, timestamp, or phone model)
2. **Waste Pictures:** 24k images -> I could not find more info for that
3. **TrashNet:** 2100 labeled images, (glass, paper, cardboard, plastic, metal, and trash)
4. **Extended TACO:** 1500 annotated images & 3000 unannotated images
5. **Wade-AI:** 1400 images, labeled
6. **UAVVaste:** It contains 772 hand-labeled aerial images of waste with over 3700 objects of one class
7. **Trash-ICRA and TrashCan:** 7212 images and 6214 annotations & 7668 images and 6706 annotations
8. **Drinking Waste:** 4800 images, labeled
9. **MJU-Waste:** 2475 indoor trash images manually annotated

**Objective:**
Compared with the existing semi-supervised model, different ways to implement semi-supervised learning are used.



### Proposal Giannis
