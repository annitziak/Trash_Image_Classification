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
### Proposal Giannis
