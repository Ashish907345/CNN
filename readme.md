# Model Performance and Analysis

## Model 1

**Target:**
- Create a lightweight model.

**Results:**
- **Parameters:** 10.8K  
- **Best Train Accuracy:** 98.64%  
- **Best Test Accuracy:** 98.38%

**Analysis:**
- The model is slightly large; it needs to be more lightweight.  
- No overfitting observed, as the gap between train and test accuracy is minimal.  
- The model shows potential for further optimization.  


---

## Model 2

**Target:**
- Add Regularization (Dropout) and Batch Normalization to increase efficiency.  
- Use Global Average Pooling (GAP) and remove the last large kernel to reduce size.

**Results:**
- **Parameters:** 6.2K  
- **Best Train Accuracy:** 98.75%  
- **Best Test Accuracy:** 96.58%

**Analysis:**
- The model is now lightweight, thanks to GAP.  
- No overfitting observed, with a minimal gap between train and test accuracy.  

---

## Model 3

**Target:**
- Increase model capacity by adding more layers at the end.  
- Incorporate image rotation (5-7 degrees) for augmentation.  
- Use a Learning Rate Scheduler for better optimization.

**Results:**
- **Parameters:** 6.45K  
- **Best Train Accuracy:** 98.8%  
- **Best Test Accuracy:** 99.41%

**Analysis:**
- The model performs well, maintaining ~99.4% accuracy over the last 5 epochs.  
- Slight underfitting is observed, which is acceptable due to challenging training with image augmentation.  

---

**Summary:**
- Each model progressively improves in terms of size, accuracy, and performance.
- Model 3 achieves the best balance between efficiency and accuracy while incorporating advanced techniques like augmentation and scheduling.
