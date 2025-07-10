# 🎼 Symphony by Sequence - Neural Networks for Music Generation

This project explores the use of sequence modeling to generate and analyze music patterns. The goal is to apply machine learning techniques—specifically RNNs and LSTMs—to learn temporal dependencies in musical sequences and generate new note predictions based on learned patterns.

This work was completed as part of the MSBA graduate program to demonstrate deep learning applications in creative domains that requires big data.

---

## 📁 Repository Structure
symphony-by-sequence/
- `code.ipynb`     | Notebook containing EDA, data processing, and modeling for music generation
- `music-output`   | Generated outputs from each model
- `report.pdf`     | Written report detailing purpose, methodology, results, and future work
- `slide-deck.pdf` | Presentation deck for data storytelling

## 🧠 Methodology

- Musical sequences were encoded as **tensorflow** tokens to represent the length, pitch, and quality of each note
- Three modeling approaches were explored, all written in PyTorch:
  - A RNN using NumPy
  - A LSTM network with tunable layers and dropout
  - A transformer utlizing a pre-trained MIDI model
- Models were trained to predict the next note in a sequence given previous inputs, resulting in music generation

---

## 📊 Evaluation

- Accuracy and loss were tracked during training
- Generated note sequences were plotted and compared to real sequences
- Manual RNN served as a baseline, while the LSTM improved temporal learning and generalization
- Transformers proved to generate the 'best' music, though it is slightly undertrained

---

## 🔮 Output

Model outputs include:
- Generated note sequences
- Visualizations of training loss and accuracy across epochs
- MIDI visualization to track music lines (i.e. melody, bassline, harmony)

- ## 🛠 Tools & Libraries

- Python (NumPy, pandas, matplotlib)
- PyTorch (LSTM model definition, training loops)
- Jupyter Notebooks (ease of collaboration)
