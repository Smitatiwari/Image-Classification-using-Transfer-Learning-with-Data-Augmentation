# Image-Classification-using-Transfer-Learning-with-Data-Augmentation

This project develops a robust deep learning classifier to distinguish between images of wild animals — specifically **arctic fox**, **polar bear**, and **walrus** — using transfer learning with **ResNet-50V2** from Keras.

## 📁 Dataset Structure
Dataset organized with train, test, and sample folders — each containing labeled images of the three animal classes.

## Objective

To build a **multiclass image classifier** that can:

- Accurately classify unseen images into one of three categories: `arctic_fox`, `polar_bear`, or `walrus`
- Generalize well across different lighting, poses, and backgrounds

## Model Architecture

- **Base Model**: `ResNet50V2` pretrained on ImageNet (via Keras Applications)
- **Transfer Learning**: Custom classification head added on top
- **Training Enhancements**:
  - **Data Augmentation**:
    - Random flipping
    - Rotation
    - Translation
    - Zoom/Scaling
  - **Callback usage**:
    - EarlyStopping
    - ModelCheckpoint

Data augmentation is applied in each epoch to boost generalization and reduce overfitting.

## Technologies Used

- Python 3
- TensorFlow / Keras
- NumPy, Matplotlib
- Jupyter Notebooks (for experimentation)

## Results

Achieved high accuracy on the test set using transfer learning and data augmentation techniques.
![image](https://github.com/user-attachments/assets/fc2ec4dd-1711-4e13-8bbd-e310d2d1b302)

