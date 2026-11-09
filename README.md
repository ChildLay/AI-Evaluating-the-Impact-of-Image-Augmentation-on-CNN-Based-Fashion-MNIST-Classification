# COMP813 Artificial Intelligence – Evaluating the Impact of Image Augmentation on CNN-Based Fashion-MNIST Classification

**Institution:** Auckland University of Technology  
**Name:** Khin Khin Maw     
**Student ID:** 24242885    

---

## Project Overview
This project investigates how different **image-augmentation strategies** affect **Convolutional Neural Network (CNN)** performance on the **Fashion-MNIST** dataset.

### Augmentation Strategies
| ID | Strategy | Description |
|----|-----------|-------------|
| A1 | No Augmentation | Baseline (no transformation) |
| A2 | Standard | Flip, Shift, Zoom, Brightness |
| A3 | Rotation Only | ±25° rotation |
| A4 | Strong | Combined, higher-intensity transformations |


### CNN Architectures
| Model | Description |
|--------|-------------|
| M1 | Baseline CNN (lightweight, 4 layers) |
| M2 | Deeper CNN (6 layers, 3 conv blocks) |
| M3 | Batch-Normalized CNN (6 layers + BatchNorm) |

Experiments were conducted under both **fixed-epoch** and **early-stopping** regimes.  
Metrics used: **Accuracy**, **Macro-F1**, and **Grad-CAM visualization**.

---

## Folder / File Structure
```
COMP813_24242885__KhinKhinMaw_CNN_BasedFashion_MNISTClassification.ipynb
    → Main Jupyter Notebook (code, figures, outputs)
requirements.txt
    → Python dependencies
README.md
    → Project overview and usage instructions
```

---

## Dependencies
Python ≥ 3.9  
tensorflow==2.19.0
numpy>=1.26
pandas>=2.2
matplotlib>=3.8
scikit-learn>=1.4 

(Exact versions listed in `requirements.txt`.)

---

##  How to Run


### 1️ Install dependencies
```bash
pip install -r requirements.txt
```

### 2️ Launch Jupyter Notebook
```bash
jupyter notebook
```

Then open:  
`COMP813_24242885__KhinKhinMaw_CNN_BasedFashion_MNISTClassification.ipynb`  
and execute all cells (**Runtime → Run All**).

or

### 3️ Launch Google Colab (Alternative)
###  Open the Notebook in Google Colab
1. Go to [Google Colab](https://colab.research.google.com/).  
2. Upload the file:  
   `COMP813_24242885__KhinKhinMaw_CNN_BasedFashion_MNISTClassification.ipynb`  
3. Once opened, make sure the runtime type is set to **GPU** (optional but faster):  
   - Click **Runtime → Change runtime type → Hardware accelerator → GPU**


### 4️ Outputs Generated
- Training and validation curves  
- Tables of Accuracy and Macro-F1  
- Confusion matrices for A1–A4  
- Activation maps (Grad-CAM)  
- Misclassified sample visualizations  

---

## Notes
- The notebook automatically downloads **Fashion-MNIST** via Keras (no external files required).  
- Model checkpoints and large files are **excluded** for submission.  
- All results are reproducible on CPU or GPU.  


---

## Acknowledgements
- TensorFlow and open-source research resources

---


**End of README**
