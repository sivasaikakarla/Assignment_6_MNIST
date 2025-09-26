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

EPOCH: 0
Loss=0.12507964670658112 Batch_id=468 Accuracy=92.21: 100%|██████████| 469/469 [00:08<00:00, 55.32it/s] 

Test set: Average loss: 0.0790, Accuracy: 9781/10000 (97.81%)

EPOCH: 1
Loss=0.051502276211977005 Batch_id=468 Accuracy=97.88: 100%|██████████| 469/469 [00:08<00:00, 54.66it/s]

Test set: Average loss: 0.0408, Accuracy: 9873/10000 (98.73%)

EPOCH: 2
Loss=0.040210530161857605 Batch_id=468 Accuracy=98.25: 100%|██████████| 469/469 [00:08<00:00, 53.33it/s]

Test set: Average loss: 0.0324, Accuracy: 9896/10000 (98.96%)

EPOCH: 3
Loss=0.021163122728466988 Batch_id=468 Accuracy=98.50: 100%|██████████| 469/469 [00:08<00:00, 53.84it/s]

Test set: Average loss: 0.0322, Accuracy: 9892/10000 (98.92%)

EPOCH: 4
Loss=0.02583286724984646 Batch_id=468 Accuracy=98.64: 100%|██████████| 469/469 [00:08<00:00, 53.01it/s] 

Test set: Average loss: 0.0308, Accuracy: 9891/10000 (98.91%)

EPOCH: 5
Loss=0.033874254673719406 Batch_id=468 Accuracy=98.72: 100%|██████████| 469/469 [00:08<00:00, 53.48it/s] 

Test set: Average loss: 0.0301, Accuracy: 9906/10000 (99.06%)

EPOCH: 6
Loss=0.03638499602675438 Batch_id=468 Accuracy=99.00: 100%|██████████| 469/469 [00:08<00:00, 53.37it/s]  

Test set: Average loss: 0.0230, Accuracy: 9931/10000 (99.31%)

EPOCH: 7
Loss=0.010519102215766907 Batch_id=468 Accuracy=99.14: 100%|██████████| 469/469 [00:08<00:00, 53.22it/s] 

Test set: Average loss: 0.0215, Accuracy: 9939/10000 (99.39%)

EPOCH: 8
Loss=0.009731670841574669 Batch_id=468 Accuracy=99.11: 100%|██████████| 469/469 [00:08<00:00, 53.85it/s] 

Test set: Average loss: 0.0212, Accuracy: 9940/10000 (99.40%)

EPOCH: 9
Loss=0.006085614208132029 Batch_id=468 Accuracy=99.12: 100%|██████████| 469/469 [00:08<00:00, 53.76it/s] 

Test set: Average loss: 0.0217, Accuracy: 9935/10000 (99.35%)

EPOCH: 10
Loss=0.032896239310503006 Batch_id=468 Accuracy=99.12: 100%|██████████| 469/469 [00:08<00:00, 53.66it/s] 

Test set: Average loss: 0.0205, Accuracy: 9940/10000 (99.40%)

EPOCH: 11
Loss=0.02950022555887699 Batch_id=468 Accuracy=99.15: 100%|██████████| 469/469 [00:08<00:00, 54.09it/s]  

Test set: Average loss: 0.0207, Accuracy: 9945/10000 (99.45%)

EPOCH: 12
Loss=0.0362660177052021 Batch_id=468 Accuracy=99.14: 100%|██████████| 469/469 [00:08<00:00, 54.30it/s]   

Test set: Average loss: 0.0205, Accuracy: 9949/10000 (99.49%)

EPOCH: 13
Loss=0.052364081144332886 Batch_id=468 Accuracy=99.14: 100%|██████████| 469/469 [00:08<00:00, 53.04it/s] 

Test set: Average loss: 0.0207, Accuracy: 9943/10000 (99.43%)

EPOCH: 14
Loss=0.006335295736789703 Batch_id=468 Accuracy=99.20: 100%|██████████| 469/469 [00:08<00:00, 53.83it/s] 

Test set: Average loss: 0.0204, Accuracy: 9943/10000 (99.43%)

