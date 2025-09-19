# SVM Classification on Fashion-MNIST

This repository contains code to apply **Support Vector Machine (SVM)** classification to the **Fashion-MNIST dataset**.  
It demonstrates how different kernels and hyperparameters (`C`, `gamma`) affect classification accuracy.

---

## Dataset
- **Fashion-MNIST** is a dataset of 70,000 grayscale images (28x28 pixels) of 10 fashion categories.  
- Training set: 60,000 images  
- Test set: 10,000 images  

Classes include:  
- T-shirt/top  
- Trouser  
- Pullover  
- Dress  
- Coat  
- Sandal  
- Shirt  
- Sneaker  
- Bag  
- Ankle boot  

---

## Project Steps
1. **Load Dataset**  
   Load Fashion-MNIST directly from `tensorflow.keras.datasets`.  

2. **Data Preprocessing**  
   - Flatten images into 1D vectors (28x28 → 784).  
   - Normalize pixel values to range [0, 1].  

3. **Visualize Samples**  
   Display 5 random sample images with their corresponding class labels.  

4. **Train SVM Classifier**  
   - Use kernels such as `linear`, `rbf`, `poly`, `sigmoid`.  
   - Experiment with different `C` values (regularization) and `gamma` values (influence of data points).  

5. **Evaluate Model**  
   - Compute accuracy on the test set.  
   - Plot accuracy across different hyperparameter values.  

6. **Visualization**  
   - Confusion matrix for classification performance.  
   - Accuracy plots across kernels and `C` values.  

---

## Requirements
Install dependencies with:
```bash
pip install numpy matplotlib scikit-learn tensorflow
```

---

## Running the Notebook
1. Open the notebook:
   ```bash
   jupyter notebook SVM.ipynb
   ```
2. Run all cells step by step to:
   - Load and preprocess data  
   - Train the SVM models  
   - Visualize results  

---

## Results
- Accuracy varies with kernel choice and hyperparameters.  
- `rbf` and `linear` kernels typically perform best on Fashion-MNIST.  
- Trade-off between **training time** and **accuracy** depending on kernel and parameter choice.  

## Submission By
- Ankit Singh 
- 2201AI47
