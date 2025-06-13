# Convolution From Scratch

**Domain:** Static-image Computer Vision  
**Project:** `01_convolution_from_scratch`
 **What it does:** Implements basic 2D convolution filters (edge‐detection, sharpen, blur) from scratch in NumPy, then trains a tiny CNN to classify synthetic images of circles, rectangles and triangles.
---

## 📂 Project Structure

```text
01_convolution_from_scratch/
├── 01_convolution_from_scratch.ipynb   ← Jupyter notebook demo
├── models/                             ← Saved model checkpoints
│   └── best_shapes_cnn.pt
├── outputs/                            ← Generated figures & previews
│   ├── convolution_demo.png
│   ├── shapes_preview.png
│   ├── qualitative_inspection.png
│   └── training_curves.png
└── README.md                           ← You are here!

📝 Overview
This notebook demonstrates:

Pure-NumPy 2D convolution on a CIFAR-10 sample

Three filter kernels:

Edge detection

Sharpening

Gaussian blur

Saving the filtered figure to
outputs/convolution_demo.png

Previewing random synthetic shapes in
outputs/shapes_preview.png

It then trains a tiny CNN on the synthetic shapes dataset and saves the best model to
models/best_shapes_cnn.pt.

⚙️ Requirements
Run within a Python 3.8+ environment with:


pip install torch torchvision \
            torchmetrics matplotlib \
            scikit-image tqdm psutil
🚀 Usage
Open 01_convolution_from_scratch.ipynb in Jupyter.

Restart & Run All (Kernel → Restart & Run All).

When complete, inspect:

Filtered figure: outputs/convolution_demo.png

Shapes preview: outputs/shapes_preview.png

Qualitative inspection: outputs/qualitative_inspection.png

Training curves: outputs/training_curves.png

Model weights: models/best_shapes_cnn.pt

🔍 Next Steps
Try additional kernels (e.g. Sobel, Laplacian)

Extend convolution to colour channels

Compare against scipy.ndimage.convolve or PyTorch’s nn.Conv2d

📜 License
MIT License — feel free to adapt or fork for your own learning.
