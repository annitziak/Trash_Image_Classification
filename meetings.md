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

##### Data Augmentation (ANNIE)
Paper: "A Comprehensive Survey of Image Augmentation Techniques for Deep Learning"
Some methods in general for images: Translation, Rotations, Intensity coloring using PCA, color shift, noise, flipping
!["Techniques used"](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*7XiKkSu6lT98NXQitQ-5MA.png)
Challenges in CV with insufficient data (e.g. image variations, class imbalance, domain shift, data remembering) <br>

Paper " Data Augmentation Using Background Replacement for Automated Sorting of LitteredWaste"
Uses just background replacement (from white background to more realistic by overlaying) -> outperform 

either by applying conventional data augmentation techniques, or by generating synthetic trash images using GANs
Used both TrashNet and TACO
operations like center cropping, flipping, rotations, brightness adjustment, translation, etc., to augment the dataset
Also generated new collages of images (combinations): overlapping and non-overlapping images -> used Gaussian-Poisson Generative Adversarial Networks (GP-GANs)
We also applied various image filters like blurring, noise filters, etc.
 we observed that the existing datasets have low frequency of images. Therefore, we investigated this issue by creating synthetic images of trash objects. Generic Generative Adversarial Networks [13] (GANs) -> discriminator, evaluator architecture were used to generate synthetic data points so as to increase the number of images to better train the models.
 Used pretrained models such as ResNet-34, ResNet-101, and VGG-16
 During synthetic image generation using GANs, we also experimented with GANs to check if the generated data of trash images can be viable for extended experiments. However, the results were not of sufficient quality to move forward with this approach.
 In the future, we intend to create a custom dataset with greater variety and number of images.

Paper : Waste Detection System Based on Data Augmentation and YOLO_EC
 Data Augmentation
 1. Non-Generative Data Augmentation  : geometric + non-geometric (on the image alter it)
 2. Generative Data Augmentation: GANs  Deep Convolutional Generative Adversarial Network ( DCGAN) with Wasserstein distance
used the HPU_WASTE dataset
data augmentation can increase the diversity of features and improve
detection accuracy
In future research, the
emphasis will be on complex backgrounds and special situations in waste image detection
to make it applicable to a wider range of classification scenarios.

other studies have used transformers e.g. vit

Data Augmentation using LLMs:
Data Perspectives, Learning Paradigms and Challenges
