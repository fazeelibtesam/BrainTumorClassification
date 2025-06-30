# 🧠 Brain Tumor Classification Using CNNs

This repository contains multiple deep learning models to classify brain tumors into **Meningioma**, **Glioma**, and **Pituitary tumor** types using MRI images. The best-performing model is a **custom-built CNN** achieving an impressive **95.11% accuracy**.

---

## 📂 Dataset

* **Classes** (after One-Hot Encoding):

  | Label | Class           | Count |
  | ----- | --------------- | ----- |
  | 0     | Meningioma      | 708   |
  | 1     | Glioma          | 1426  |
  | 2     | Pituitary Tumor | 930   |

---

## 🏗️ Models Compared

| Model Name                  | Description                                                                         |
| --------------------------- | ----------------------------------------------------------------------------------- |
| **MODEL1: MobileNetV2**     | Lightweight CNN, pretrained on ImageNet, good for small datasets and fast inference |
| **MODEL2: ResNet50**        | Deep residual network, ImageNet pretrained, better for deeper feature learning      |
| **MODEL3: EfficientNetB0**  | Balanced in speed and accuracy, state-of-the-art architecture                       |
| **MODEL4: Custom CNN** ✅    | Built from scratch, fast experimentation, fine-tuned layers – **Best Performance**  |
| **MODEL5: Custom CNN + BN** | Same as above but with added `BatchNormalization` layers for better generalization  |

---

## ✅ Best Performing Model: Custom CNN

* Built from scratch using `Keras`
* Fine-tuned with additional optimizations
* Accuracy: **95.11%**
* Output layer: `Dense(3, activation='softmax')`

---

## 📊 Results

| Model                    | Accuracy   |
| ------------------------ | ---------- |
| MobileNetV2              | \~88%      |
| ResNet50                 | \~91%      |
| EfficientNetB0           | \~92.5%    |
| **Custom CNN (Model 4)** | **95.11%** |
| Custom CNN + BN          | \~93%      |

---

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/fazeelibtesam/brain-tumor-classification-cnn.git
cd brain-tumor-classification-cnn

# Create and activate a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. **Prepare Dataset**
   Ensure the dataset is structured as:

   ```
   dataset/
   ├── glioma/
   ├── meningioma/
   └── pituitary/
   ```

2. **Train a Model**
   Modify and run the desired script:

   ```bash
   python train_custom_cnn.py  # For Model 4
   ```

3. **Evaluate the Model**

   ```bash
   python evaluate_model.py
   ```

---

## 📈 Future Work

* Implement advanced data augmentation
* Test with more EfficientNet variants (B1–B3)

---

## 📄 License

This project is licensed under the [Apache2.0 License](LICENSE).

---

## 🙌 Acknowledgments

* MRI Dataset from Cheng, Jun (2017)
* Pretrained models via `keras.applications`

---

## 🤝 Contact for Collaboration

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

I'm open to feedback, collaboration, or ideas for improvements. Feel free to reach out!

* 📧 Email: [ibtesamfazeel@gmail.com](mailto:ibtesamfazeel@gmail.com)
* 💼 LinkedIn: [https://linkedin.com/in/fazeel-ibtesam](https://linkedin.com/in/fazeel-ibtesam)
* 🐙 GitHub: [https://github.com/fazeelibtesam](https://github.com/fazeelibtesam)


Feel free to fork, star ⭐, and follow for updates!

---
