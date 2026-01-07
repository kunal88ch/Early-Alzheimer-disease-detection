# Early Alzheimer's Disease Detection

## 📌 Project Overview
Alzheimer's disease is a progressive neurologic disorder that causes the brain to shrink (atrophy) and brain cells to die. Early detection is crucial for managing the disease and improving the quality of life for patients. 

This project aims to **develop and evaluate a Convolutional Neural Network (CNN)-based model** to detect Alzheimer’s disease from brain MRI images. By leveraging deep learning, we can provide a faster, cost-effective, and reliable alternative to traditional diagnostic methods.

### 🎯 Key Objectives
- **Early Detection**: Identify signs of Alzheimer's at early stages (Mild Demented).
- **Classification**: Differentiate between four classes of MRI scans:
    1.  **Non-Demented**
    2.  **Very Mild Demented**
    3.  **Mild Demented**
    4.  **Moderate Demented**
- **User-Friendly Interface**: A simple web application for users to upload MRI images and get instant predictions.

## 🧠 The Solution
We utilize a Deep Learning model trained on MRI datasets to classify brain scans. Structurally, the project consists of:
1.  **Data Preprocessing**: Handling MRI images and augmenting them for better training.
2.  **CNN Model**: A custom Convolutional Neural Network trained to recognize patterns associated with different stages of dementia.
3.  **Streamlit Web App**: A frontend interface where users can upload an image and view the model's prediction along with a confidence score.

## 🛠️ Tech Stack
-   **Language**: Python 3.9+
-   **Deep Learning**: TensorFlow, Keras
-   **Web Framework**: Streamlit
-   **Image Processing**: OpenCV, PIL (Pillow), NumPy
-   **Visualization**: Matplotlib (in notebook), Streamlit Lottie

## 🚀 Getting Started

### Prerequisites
-   Python installed on your system.
-   Git installed on your system.

### Installation

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/kunal88ch/Early-Alzheimer-disease-detection.git
    cd Early-Alzheimer-disease-detection
    ```

2.  **Create a Virtual Environment (Optional but Recommended)**
    ```bash
    python -m venv venv
    # On Windows
    .\venv\Scripts\activate
    # On macOS/Linux
    source venv/bin/activate
    ```

3.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

### 🏃‍♂️ specific Usage

#### 1. Generate the Model
The web application requires a trained model file (`alzheimer_model.h5`). If this file is not present in the directory, you need to generate it by running the Jupyter Notebook:
-   Open `Alzeihmer_Disease_Detection_and_Classification.ipynb`.
-   Run all the cells to train the model.
-   Ensure `alzheimer_model.h5` is saved in the project root.

#### 2. Run the Web App
Once the dependencies are installed and the model is ready, run the Streamlit application:
```bash
streamlit run app.py
```
This will open the application in your default web browser (usually at `http://localhost:8501`).

#### 3. Using the App
-   Click on **"Browse files"** to upload a brain MRI image (JPG or PNG).
-   The app will display the uploaded image.
-   The model will process the image and output the **Predicted Class** (e.g., "VeryMildDemented") and a **Confidence Score**.

## 📂 Project Structure
```
├── Alzeihmer_Disease_Detection_and_Classification.ipynb # Jupyter Notebook for training
├── app.py                  # Main Streamlit Web Application
├── alzheimer_model.h5      # Trained Model (Generated after training)
├── requirements.txt        # Python dependencies
├── styles.css              # Custom CSS for the web app
├── images/                 # Assets for the web app
├── pics/                   # Sample images
├── Alzheimer_disease_report.pdf # Project Report
└── README.md               # Project Documentation
```

## 🤝 Contribution
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## 📄 License
This project is open-source and available for educational and research purposes.
