[README.md](https://github.com/user-attachments/files/21704783/README.md)
# 🌱 Crop Classifier

This is a **Streamlit** web application that classifies crop images into their respective categories using a fine-tuned **ResNet18** model.

## 📌 Features
- Upload an image of a crop (`.jpg`, `.jpeg`, `.png`)
- Model predicts the crop type
- Built with PyTorch and Streamlit

---

## 📂 Project Structure
```
.
├── crop_classifier.py        # Main Streamlit app
├── crop_classifier_model.pkl # Trained model & class mappings
├── Analysis.ipynb            # Model training and evaluation notebook
└── README.md                 # Project documentation
```

---

## ⚙️ Installation

1. **Clone the repository**  
```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
```

2. **Create a virtual environment (optional but recommended)**  
```bash
python -m venv venv
source venv/bin/activate  # On Mac/Linux
venv\Scripts\activate     # On Windows
```

3. **Install dependencies**  
```bash
pip install -r requirements.txt
```
*(If `requirements.txt` is missing, install manually:)*  
```bash
pip install streamlit torch torchvision pillow joblib
```

---

## 🚀 Usage

Run the Streamlit app:
```bash
streamlit run crop_classifier.py
```

---

## 📖 How It Works
- Loads a trained **ResNet18** model from `crop_classifier_model.pkl`
- Preprocesses uploaded images:
  - Resize to `224x224`
  - Normalize with ImageNet stats
- Predicts the crop class and displays it to the user

---

## 🖼 Example

**Uploaded Image:**  
*(User uploads a crop image)*  

**Prediction:**  
```
Predicted Crop: Wheat
```

---

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
