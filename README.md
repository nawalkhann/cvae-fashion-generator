# CVAE Fashion Generator 👗

A **Convolutional Variational Autoencoder (CVAE)** built in PyTorch to learn, compress, and generate fashion clothing images.

**Course:** MGT488 – Advanced Deep Learning
**Team:** Fatima, Nawal, Uswa
**Semester:** 7th-A
**Submitted to:** Sir Saeed ur Rehman

## 🎯 Project Overview
This project builds a CVAE that:
1. Learns the visual features of fashion clothing images
2. Compresses images into a latent space representation
3. Reconstructs and generates new synthetic fashion images from that latent space

## 🧰 Tech Stack
- Python
- PyTorch / Torchvision
- NumPy, Matplotlib, PIL
- Kaggle API (dataset acquisition)
- Google Colab (GPU training)

## 📂 Project Structure
```
├── CVAE_Fashion_Generator.ipynb   # Main notebook
├── requirements.txt               # Dependencies
└── README.md
```

## 🔬 Workflow
1. **Dataset Acquisition & GPU Setup** – Download fashion dataset via Kaggle API, configure GPU
2. **Data Preprocessing** – Resize, normalize, and split images into train/test
3. **Custom Dataset & DataLoader** – Build PyTorch `Dataset` class for image loading
4. **Model Architecture** – Convolutional encoder-decoder VAE with reparameterization trick
5. **Training** – Adam optimizer, combined MSE + KL divergence loss
6. **Evaluation & Generation** – Reconstruct test images, generate synthetic samples, latent space interpolation
7. **Experimentation** – Compare results across image resolutions (64×64, 128×128, 256×256)

## 🚀 How to Run
1. Open the notebook in Google Colab
2. Upload your `kaggle.json` API key when prompted
3. Run cells sequentially (Runtime → GPU recommended)

## 📊 Results
The model reconstructs fashion images and generates new synthetic samples via random latent vectors, with latent space interpolation demonstrating smooth transitions between garment styles.
