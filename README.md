# 🖼️ Image Classification using CNN  
## 🌟 Overview  
This project applies **Computer Vision** techniques, specifically **Convolutional Neural Networks (CNNs)**, for image classification. Using the CIFAR-10 dataset, the goal was to design, train, and optimize a CNN model with a focus on hyperparameter tuning and performance evaluation. The implementation leveraged **Keras**, an open-source neural network library, for building the model.  

[🎥 Watch the YouTube Demo](https://www.youtube.com/watch?v=x7YUDexpYo0)  

---

## 🔍 Introduction  
In this project, we explored the development of a CNN for **image classification** using the **CIFAR-10 dataset**, consisting of 60,000 images across 10 categories.  
Key objectives:  
- Build and optimize a CNN architecture.  
- Experiment with hyperparameters and evaluate their impact.  
- Use data augmentation and other techniques to improve performance.  

---

## 🗂️ Dataset  
- **Source**: [CIFAR-10 on Kaggle](https://www.kaggle.com/c/cifar-10/)  
- **Classes**: 10 categories (airplanes, cars, birds, cats, deer, dogs, frogs, horses, ships, and trucks).  
- **Preprocessing**: Normalized pixel values to the range [0, 1].  

---

## ⚙️ Methodology  
### First Experimentation (78% Accuracy)  
- **Model Architecture**:  
  - 3 Convolutional Layers with increasing filters (32, 64, 128).  
  - Batch Normalization, MaxPooling, Flatten, and Dense Layers.  
  - Dropout (30%) for regularization.  
- **Optimizer**: Adam with a learning rate of 0.001.  
- **Result**: Achieved 78% accuracy on the test set.  

---

### Second Experimentation (79.5% Accuracy)  
- **Enhancements**:  
  - Added a 4th convolutional layer with 256 filters.  
  - Increased Dense layer size to 512 neurons.  
- **Challenges**: Higher computational cost (training time increased to 13 hours).  
- **Result**: Accuracy improved to 79.5%.  

---

### Third Experimentation (87% Accuracy)  
- **Techniques**:  
  - Increased training epochs to 50.  
  - Introduced **data augmentation** (random shifts and flips) to improve generalization.  
- **Result**: Accuracy improved to 87%.  

---

## 🔬 Hyperparameter Exploration  
1. **Learning Rate**:  
   - Optimal: 0.0001 (accuracy = 75.32%).  
   - Higher or lower rates led to reduced performance.  

2. **Dropout Rate**:  
   - Optimal: 0.2 (accuracy = 74.79%).  
   - Variations showed competitive performance but lower robustness.  

3. **Optimizers**:  
   - Best: Adam (accuracy = 76.91%).  
   - Others (SGD, RMSprop, etc.) had lower accuracy.  

4. **Loss Functions**:  
   - Best: Binary Crossentropy (accuracy = 75.25%).  
   - Categorical Crossentropy also showed competitive results.  

---

## ✅ Conclusion  
This project highlights the critical role of CNNs in image classification tasks:  
- Achieved a final test accuracy of **87%** using an optimized architecture and data augmentation.  
- Explored hyperparameters to find optimal settings for learning rate, dropout rate, and optimizer choice.  
- Overcame computational challenges, such as overfitting and long training times, through regularization techniques.

---

## 📚 References  
- [CIFAR-10 Dataset](https://www.kaggle.com/c/cifar-10/)  
- [Convolutional Neural Networks Video by Codebasics](https://www.youtube.com/watch?v=zfiSAzpy9NM)  
- [Keras Documentation](https://keras.io/)  
- [Demo Source Code and Training Video](https://youtu.be/J1jhfAw5Uvo)   
