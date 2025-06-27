## Libraries required
- scikit-learn
- numpy
- matplotlib
- seaborn
- imageio
- scikit-image

## How It Works

### 1. Data Preparation
- Unzips and loads image files from labeled folders.
- Resizes all images to **64×64** and flattens them to 1D vectors.
- Normalizes pixel values to `[0, 1]`.

### 2. Model Training

#### Random Forest:
- Trained using **GridSearchCV** for hyperparameter tuning.
- Best model selected based on cross-validation accuracy.

#### SVM:
- Trained using default `SVC()` settings for comparison.

### 3. Evaluation
- Accuracy, Precision, Recall, F1 Score calculated on test set.
- Confusion matrix plotted with Seaborn.
- Feature importance visualized for Random Forest.

### 4. Prediction
- A utility function allows class prediction for any new image.

---

## 📊 Results Summary

**Model**               **Accuracy**        **F1 Score** 
Random Forest              74.2%               72.2%    
SVM                        72.6%               69.9%    

**Random Forest** slightly outperformed SVM and provides feature importance for interpretability.



## Example Usage
# Predict a single image
predicted_class = predict_image("/content/images/images/sunflower/image_0044.jpg", best_rf)
print("Predicted class:", predicted_class)

