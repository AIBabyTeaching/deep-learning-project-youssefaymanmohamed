# Traffic Sign Classification

This repository contains code for training and evaluating two models for traffic sign classification. The first model is a custom Convolutional Neural Network (CNN), while the second model uses transfer learning with a pre-trained ResNet50 model.

## Models Overview

### Custom CNN (Model 1)

- **Architecture:**
  - Convolutional Neural Network with multiple convolutional layers, max pooling, and dense layers.
  
- **Training Dynamics (Epochs 1-10):**
  - Training Loss: 0.0141
  - Training Accuracy: 99.6%
  - Validation Loss: 0.1093
  - Validation Accuracy: 97.4%
  
- **Test Performance:**
  - Test Accuracy: 95.18%
  - Test Loss: 0.2587

### Transfer Learning with ResNet50 (Model 2)

- **Architecture:**
  - Transfer learning using a pre-trained ResNet50 model.

- **Training Dynamics (Epochs 1-5):**
  - Training Loss: 0.0230
  - Training Accuracy: 99.45%
  - Validation Loss: 0.2687
  - Validation Accuracy: 94.58%
  
- **Test Performance:**
  - Test Accuracy: 94.58%
  - Test Loss: 0.2687

## Comparison and Recommendations

- **Accuracy:**
  - The first model achieves slightly higher accuracy on the test set (95.18%) compared to the second model (94.58%).

- **Training Dynamics:**
  - The first model shows a steady decrease in training and validation loss over 10 epochs, indicating effective training.
  - The second model, using transfer learning, achieves high training accuracy but seems to have a higher validation loss, suggesting potential overfitting or the need for further fine-tuning.

- **Architecture and Training Time:**
  - The first model uses a custom CNN architecture and appears to train faster (epochs complete in around 42 seconds), while the second model takes longer (epochs complete in around 20 seconds).

## Recommendations

- **Considerations for Model 1:**
  - Investigate further into the features learned by the custom CNN and potentially explore hyperparameter tuning.

- **Considerations for Model 2:**
  - For the second model, given the use of transfer learning, consider fine-tuning the model by adjusting learning rates or using differential learning rates for different layers to improve validation performance.

- **General Recommendations:**
  - Evaluate both models on a broader test set to ensure a fair comparison.
  - Consider ensemble methods if applicable, combining predictions from both models for potentially improved performance.


