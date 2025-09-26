# MNIST Classifier: Achieving 99.4% Accuracy with <8K Parameters

This repository documents the process of building a lightweight **Convolutional Neural Network (CNN)** to classify the **MNIST dataset**, adhering to strict performance and size constraints.

---

## Target

The objective was to design a model that achieves the following:

- **Test Accuracy**: Consistently > **99.4%** in the final epochs  
- **Epochs**: Training completed in ≤ **15 epochs**  
- **Model Size**: Less than **8,000 parameters**  

---

## Building Steps


1. **Model_1**  
   - Build a minimal, lightweight model under 8k parameters.  
   - Train for ≤ 15 epochs to verify setup and establish baseline performance.  

2. **Model_2**  
   - Address underfitting by introducing padding, deeper conv blocks.  
   - Staying under the 8k parameter constraint.  

3. **Model_3**  
   - Refine the architecture.  
   - Introduce a **Learning Rate Scheduler** (StepLR) to break accuracy plateaus.  
   - Target consistent >99.4% accuracy.  

---
### Model Results (Model_1)

EPOCH: 12 | Test Accuracy: 98.99%
EPOCH: 13 | Test Accuracy: 98.92%
EPOCH: 14 | Test Accuracy: 99.01%

### Model Results (Model_2)

EPOCH: 12 | Test Accuracy: 99.06%
EPOCH: 13 | Test Accuracy: 99.05%
EPOCH: 14 | Test Accuracy: 98.99%

### Model Results (Model_3)

![Model_3](images/model3_training.png](https://drive.google.com/file/d/1QsUg-plz8ZN8t3FZDiMfTI9X-iOjSgGR/view?usp=sharing)

### Training results

![GRAPH]([images/model3_training.png](https://drive.google.com/file/d/1a0t0otp-jivQI6_1twzfuMRFZenmBaOp/view?usp=sharing))


