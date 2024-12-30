# 1.Predicting Waste Through Image Recognition

### TrashNet Dataset Overview
[Trashnet](https://universe.roboflow.com/polygence-project/trashnet-a-set-of-annotated-images-of-trash-that-can-be-used-for-object-detection/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true)

- **Content**: The dataset comprises 2,527 images categorized into six classes: cardboard, glass, metal, paper, plastic, and trash.
- Previous work includes:
  **Convolutional Neural Networks (CNNs)**:
    - *AlexNet*: Modifying the AlexNet architecture, one study achieved a test accuracy of approximately 79.94% when combined with an SVM classifier.
        
        [CS230](https://cs230.stanford.edu/projects_spring_2020/reports/38847029.pdf?utm_source=chatgpt.com)
        
    - *ResNet-50*: Utilizing transfer learning with ResNet-50, another approach reached a classification accuracy of 92.4%.
        
        [ArXiv](https://arxiv.org/abs/2011.01353?utm_source=chatgpt.com)
        
- **DenseNet Architectures**:
    - Implementations of DenseNet121 and DenseNet169, optimized with the Adam optimizer and data augmentation techniques, have demonstrated superior test accuracies compared to other models.

### Current Research Landscape

- **Deep Learning Models**: Convolutional Neural Networks (CNNs) have been extensively employed for waste classification tasks. For instance, a study utilizing a modified ResNet-50 architecture achieved a classification accuracy of 92.4% on the TrashNet dataset.
    
    [ArXiv](https://arxiv.org/abs/2011.01353?utm_source=chatgpt.com)
    
- **Transfer Learning**: Pre-trained models like EfficientNet-B0 have been fine-tuned for waste classification, demonstrating high efficiency and accuracy. One such approach reported comparable accuracy to EfficientNet-B3 while requiring significantly fewer computational resources.
    
    [MDPI](https://www.mdpi.com/2071-1050/14/12/7222?utm_source=chatgpt.com)
    
    ## Potential Literature Gap
    
    **Multi-Label Classification Challenges**: Although progress has been made, accurately classifying images containing multiple waste items is still complex. Developing models that can effectively handle overlapping objects and varying spatial arrangements is an ongoing research area.
    
# 2. Sentiment Analysis Example (or another more NLP based task)
    
 ### **Datasets options**
    
   ### IMDb Movie Reviews**:
        - **Content**: The dataset consists of 50,000 movie reviews labeled as positive or negative. The data is evenly split into training and testing sets, with 25,000 reviews each.
        - **Challenges**: Sentences vary in length, structure, and complexity, presenting challenges for sequential models like RNNs and Transformers.
        - [Link to Dataset](https://ai.stanford.edu/~amaas/data/sentiment/)

        
   ### **Yelp Reviews Dataset**

   #### **Content**
   The Yelp Reviews Dataset contains text reviews and metadata from Yelp, including ratings on a scale of 1 to 5 stars.
    
   - **Features**:
   - Text reviews for businesses across various categories (restaurants, shops, services).
   - Ratings (1–5 stars)
   - Metadata: business category, location, and review time.
    
   #### **Challenges**
   Handling imbalanced classes as most reviews are either very positive or very negative.
   Managing domain-specific language (e.g., slang, regional terms).
    
   #### **Models**
   **LSTM**: Analyze sequential dependencies in review text.
   **GRU**: A lighter alternative for faster processing.
   **Transformers**: Use pre-trained models like RoBERTa for nuanced understanding.
    
   #### **Dataset Link**
   [Yelp Dataset](https://www.yelp.com/dataset)
        
   ## Models we can use for this task 
   LSTM
   GRU
   Transformers - can be pretrained e.g. roberta etc. (can be found in huggingface website)
        
   Model comparison
    

# **3. Medical Image Classification (CNN and Transformers)**

- **Dataset**: ChestX-ray8, Brain tumor multimodal image  / also look at kaggle for many datasets
- **Task**: Detect lung diseases from chest X-ray images / other diseases
- **Baseline Method**: Use CNN (e.g., ResNet or EfficientNet) etc. 
- **Improvement Strategies**:
    - Introduce Transformer-based models like Vision Transformers (ViT) for better global feature representation.
    - Explore data augmentation techniques such as rotation and contrast adjustment.
    - Use Grad-CAM to visualize areas of interest and refine the model.

# 4. Traffic predictions?
