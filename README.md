**First Model:**
</br>

**Architecture:**</br>

- Convolutional Neural Network (CNN) with multiple convolutional layers followed by dense layers.</br>
- Max pooling layers for down-sampling.</br>
- Flatten layer before the dense layers.</br>

**Training Dynamics (Epochs 1-10):**</br>

- Training Loss: 0.0141</br>
- Training Accuracy: 99.6%</br>
- Validation Loss: 0.1093</br>
- Validation Accuracy: 97.4%</br>

**Test Performance:**


- Test Accuracy: 95.18%
- Test Loss: 0.2587
- Second Model:
- Architecture:

**Transfer learning using a pre-trained ResNet50 model.**</br>

**Training Dynamics (Epochs 1-5):**
</br>

- Training Loss: 0.0230</br>
- Training Accuracy: 99.45%</br>
- Validation Loss: 0.2687</br>
- Validation Accuracy: 94.58%</br>
**Test Performance:**</br>

- Test Accuracy: 94.58%</br>
- Test Loss: 0.2687</br>

**Comparison:**</br>

**Accuracy:**</br>

- The first model has a slightly higher accuracy on the test set (95.18%) compared to the second model (94.58%).
</br>

**Training Dynamics:**</br>

- The first model shows a steady decrease in training and validation loss over 10 epochs, indicating effective training.</br>
- The second model, using transfer learning, achieves a high training accuracy but seems to have a higher validation loss, suggesting potential overfitting or the need for further fine-tuning.</br>
**Architecture:**</br>

- The first model uses a custom CNN architecture, while the second model employs a more complex architecture based on a pre-trained ResNet50 model.
Training Time:
</br>
- The first model appears to train faster (epochs complete in around 42 seconds), while the second model takes longer (epochs complete in around 20 seconds).
