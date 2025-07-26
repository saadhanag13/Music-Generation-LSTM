## 🎼 Music Generation with LSTM

A deep learning-based project that generates classical-style music using Long Short-Term Memory (LSTM) networks trained on MIDI datasets.

## 📂 Project Highlights
- Built using TensorFlow/Keras
- Trained on a Kaggle MIDI dataset
- Generates note sequences in MIDI format
- Visualizes predictions and training stats

## 🧠 Model Overview
- One-hot encoding of notes
- Sequential LSTM layers with Dropout
- Dense output layer for note prediction

## 🚀 Model Architecture

<img width="2140" height="740" alt="Model Arch" src="https://github.com/user-attachments/assets/6e396099-9696-43c4-a070-71a387269e23" />

The model is designed using a **Sequential LSTM architecture** for next-note prediction in music sequences.

| Layer (type)        | Output Shape | Param # |
|---------------------|--------------|---------|
| LSTM                | (None, 256)  | 271,360 |
| Dropout             | (None, 256)  | 0       |
| Dense               | (None, 128)  | 32,896  |
| Activation (ReLU)   | (None, 128)  | 0       |
| Dense               | (None, 88)   | 11,352  |
| Activation (Softmax)| (None, 88)   | 0       |
| **Total Parameters**|              | **315,608** |

### 📌 Layer Details:
- LSTM Layer: 256 units to capture temporal dependencies in music sequences

- Dropout Layer: Prevents overfitting

- Dense Layers: Fully connected layers for mapping LSTM output to 88-note vocabulary

- Activation Functions: relu and softmax used for non-linearity and output probability distribution

## 📊 Training Results
- Loss Function: categorical_crossentropy

- Optimizer: Adam

- Epochs Trained: 50

- Batch Size: 64

- Final Training Loss: ~0.17

- Model Convergence: The model shows steady convergence across epochs with minimal overfitting observed.

## 📉 Loss Curve:
The graph below shows the model loss decreasing steadily, indicating good learning progression:

<img width="500" height="350" alt="training_loss_curve" src="https://github.com/user-attachments/assets/a0e77426-525e-4e55-a5f5-bde7439fac58" />

## 📦 Installation

### Clone the repo
- git clone https://github.com/yourusername/Music-Generation-LSTM.git
- cd Music-Generation-LSTM

### Install dependencies
pip install -r requirements.txt

## 🧑‍💻 Author
### Saadhana Ganesa Narasimhan
MSc Graduate | Aspiring AI/ML Engineer | Passionate about real-world deep learning applications

### 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://saadhanag13.github.io/MyResume/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/saadhana-ganesh-45a50a18b/)



