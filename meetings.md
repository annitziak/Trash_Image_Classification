## 16/01/2025

Model architectures: <br>
1. CNNs - (bn ,rc, downsampling)
2. ViT - Vision Transformers
3. ResNet
4. AlexNet?
5. EfficientNet?
6. DenseNet


Ideas
1. Image preprocessing ( denoising, colors, normalization, scaling, rotations, saturations etc)
2. Transfer learning
3. Semi supervised learning ? 

Potentially:
Multi-Label Classification Challenges

# DATASETS
## TACO Dataset
- **Purpose:** Detecting litter in natural and urban environments.
- **Image Content:** Complex scenes with multiple, often **overlapping** items and ** more real-world examples**
- **Annotations:** Includes bounding boxes and masks for object detection and segmentation.
- **Use Cases:** Suitable for real-world applications requiring precise item localization, such as autonomous cleaning robots and environmental monitoring.
- **Dataset Size and Diversity:** Large and varied, representing diverse trash types and environmental conditions.

## TrashNet Dataset
- **Purpose:** Classifying types of trash for recycling automation.
- **Image Content:** Simpler, isolated items photographed against a** plain background.** <- easier
- **Annotations:** Class labels for basic material types (e.g., glass, paper, plastic).
- **Use Cases:** Ideal for classification tasks in controlled environments, such as sorting facilities.
- **Dataset Size and Composition:** Smaller and less complex, focusing on basic classification without localization.

## 21/01/2025
1. feature based eg. texture, shape, color, reflectness, transparency etc → compare with a neural GIANNIS 
2. data augmentation + images → white background, noisy etc. ANNIE 
3. semi supervised VASILIS
4. multi object detection* → difficult
5. comparison taco/trashnet?

