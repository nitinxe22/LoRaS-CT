# LoRaS-CT
LoRaS-CT: A Structured Low-Rank Sparse Multi-Head Self-Attention-Based Hybrid CNN-Transformer with Cross-Model Knowledge Distillation for Efficient Contextual Representation Learning in Histopathology

# LoRaS-CT

LoRaS-CT is a hybrid CNN-Transformer framework for efficient
histopathology image classification using low-rank sparse multi-head
attention.


## Notebooks
| Notebook | Description |
|---|---|
| `Kather5K.ipynb` | Kather5k experiments |
| `CRC7K.ipynb` | CRC7k experiments |
| `BreakHis.ipynb` | BreakHis experiments |
| `LC25000.ipynb` | LC25000 experiments |
| `NCT100K.ipynb` | NCT100k experiments |
| `KD-WithoutKD_LC-NCT.ipynb` | KD and without-KD experiments |
| `LoRaS-CT_KD_vs_NoKD.ipynb` | KD vs. without-KD comparison |
## Requirements
- Python 3.x
- PyTorch 2.6.0
- TorchVision 0.21.0
- CUDA-enabled GPU
## Usage
Download the required datasets, update the dataset paths in the
corresponding notebooks, and run the notebooks sequentially.
## Reproducibility
The notebooks contain the experimental pipeline used for the results
reported in the manuscript.
