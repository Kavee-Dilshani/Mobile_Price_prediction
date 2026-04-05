# 📱 Mobile Price Prediction using ANN (TensorFlow)

## 📌 Project Overview

I wants to predict whether a mobile phone falls into a **high (1)** or **low (0)** price category based on its features such as RAM, internal memory, and other specifications.

This project builds a **Simple Artificial Neural Network (ANN)** using TensorFlow to learn the relationship between mobile features and price range.

---

## 📂 Dataset

* Input: CSV file containing mobile phone specifications
* Output: Binary label

  * **1 → High price**
  * **0 → Low price**

---

## ⚙️ Steps Performed

### 1. Load Dataset

* Read the CSV file using `pandas`
* Separate features (X) and target (y)

### 2. Data Splitting

* Split dataset into:

  * **75% Training Data**
  * **25% Testing Data**
* Used `train_test_split` from `sklearn`

---

## 🧠 ANN Model Architecture

The model is built using TensorFlow/Keras with the following structure:

* **Input Layer**
* **Hidden Layer 1** → 8 neurons, activation = ReLU
* **Hidden Layer 2** → 4 neurons, activation = ReLU
* **Output Layer** → 1 neuron, activation = Sigmoid

---

## 🔧 Model Compilation

* **Loss Function**: `binary_crossentropy`
* **Optimizer**: `sgd`
* **Metrics**: `accuracy`

---

## 🚀 Model Training

* **Epochs**: 100
* **Batch Size**: 32

The model is trained on the training dataset to learn patterns.

---

## 💾 Saving Model Weights

After training, the model weights are saved using:

```python
model.save_weights("model_weights.h5")
```

This allows reuse of the trained model for future predictions without retraining.

---

## 📊 Expected Outcome

* The model predicts whether a mobile phone belongs to:

  * **High price range**
  * **Low price range**
* Helps in decision-making for pricing new mobile products.

---

## 🛠️ Technologies Used

* Python
* TensorFlow / Keras
* Pandas
* Scikit-learn

---

## 📌 Conclusion

This project demonstrates how an ANN can be used for **binary classification** problems like price prediction. The trained model can assist Nimal in making **data-driven pricing decisions** in a competitive market.

---
