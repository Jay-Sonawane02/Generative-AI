# Fashion MNIST Neural Network Classifier

This project implements a **Neural Network using TensorFlow/Keras** to classify clothing images from the **Fashion-MNIST dataset**.

The goal is to train a model that can recognize different types of clothing from grayscale images.

---

## Dataset

Fashion-MNIST is a dataset of **70,000 grayscale images** of clothing items.

* **Training images:** 60,000
* **Test images:** 10,000
* **Image size:** 28 × 28 pixels
* **Number of classes:** 10

### Classes

| Label | Item          |
| ----- | ------------- |
| 0     | T-shirt / Top |
| 1     | Trouser       |
| 2     | Pullover      |
| 3     | Dress         |
| 4     | Coat          |
| 5     | Sandal        |
| 6     | Shirt         |
| 7     | Sneaker       |
| 8     | Bag           |
| 9     | Ankle Boot    |

---

## Model Architecture

The neural network used in this project consists of:

* **Input Layer:** 784 neurons (flattened 28×28 image)
* **Dense Layer:** ReLU activation
* **Dropout Layer:** prevents overfitting
* **Dense Layer:** ReLU activation
* **Dropout Layer**
* **Output Layer:** Softmax activation (10 classes)

---

## Training Details

* **Optimizer:** Adam
* **Loss Function:** Categorical Crossentropy
* **Batch Size:** 64
* **Epochs:** 10

---

## Results

The model achieves approximately **88–90% accuracy** on the test dataset.

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

## How to Run

Install required libraries:

```
pip install tensorflow numpy matplotlib scikit-learn
```

Run the notebook:

```
fashion_mnist.ipynb
```

---

## Author

Jay Sonawane
IIT Bombay
