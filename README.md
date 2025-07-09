
# 🌿 Plant Disease Classification using CNN

This project uses Deep Learning to classify images of plant leaves into different disease categories. It leverages a custom CNN model built with TensorFlow/Keras and trained on a labeled dataset of plant leaf images.

---

## 📌 Features

- 📁 **Image Loading:** Efficient loading of images from directories using `image_dataset_from_directory`
- 🔀 **Custom Dataset Splitting:** Custom Python logic to split dataset into training, validation, and test sets
- 🖼️ **Visualization:** Displayed labeled sample images to validate dataset integrity
- 🧠 **CNN Model:** Built a convolutional neural network with Conv2D, MaxPooling2D, Flatten, and Dense layers
- ⚙️ **Model Compilation:** Compiled using `Adam` optimizer and `categorical_crossentropy` loss
- 🏋️‍♂️ **Training & Evaluation:** Trained and evaluated the model using accuracy and loss metrics
- 💾 **Model Saving:** Exported the trained model as a `.keras` file for later use

---

## 🧪 Model Architecture

```python
Sequential([
    Rescaling(1./255),
    Conv2D(16, 3, activation='relu'),
    MaxPooling2D(),
    Conv2D(32, 3, activation='relu'),
    MaxPooling2D(),
    Conv2D(64, 3, activation='relu'),
    MaxPooling2D(),
    Flatten(),
    Dense(128, activation='relu'),
    Dense(num_classes)
])
```

---

## 🧬 Tech Stack

- Python 🐍
- TensorFlow & Keras
- Matplotlib for visualization
- Jupyter Notebook (for development)

---



## 🚀 Getting Started

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/plant-disease-classifier.git
   cd plant-disease-classifier
   ```

2. Install dependencies:
   ```bash
   pip install tensorflow matplotlib
   ```

3. Run the notebook:
   ```bash
   jupyter notebook model.ipynb
   ```

---

## ✅ Output

- Model trained with high accuracy on training and validation datasets
- Successfully classified plant leaf diseases across multiple categories

---

## 📌 Future Improvements

- Deploy the model via a web or mobile app
- Use transfer learning with pre-trained models (e.g., MobileNetV2)

---

## 📬 Contact

Created by **Anshu**  
Feel free to reach out or contribute!
