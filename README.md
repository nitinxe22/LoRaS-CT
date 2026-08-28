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

## Trained Weights

Trained model weights are available in the [Releases](https://github.com/nitinxe22/LoRaS-CT/releases/tag/weights-v1) section:

| Model | Dataset | Size | Download |
|---|---|---|---|
| LoRaS-CT | LC25000 | 111 MB | [Download](https://github.com/nitinxe22/LoRaS-CT/releases/download/weights-v1/LC25000_LoRaS-CT_weights.pth) |
| MHA-Net | LC25000 | 128 MB | [Download](https://github.com/nitinxe22/LoRaS-CT/releases/download/weights-v1/LC25000_MHA-Net_baseline_weights.pth) |
| LoRaS-CT | NCT100k | 111 MB | [Download](https://github.com/nitinxe22/LoRaS-CT/releases/download/weights-v1/NCT100k_LoRaS-CT_weights.pth) |
| MHA-Net | NCT100k | 128 MB | [Download](https://github.com/nitinxe22/LoRaS-CT/releases/download/weights-v1/NCT100k_MHA-Net_baseline_weights.pth) |

### Loading a checkpoint
```python
import torch
model.load_state_dict(torch.load('LC25000_LoRaS-CT_weights.pth', map_location='cpu'))
```
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
