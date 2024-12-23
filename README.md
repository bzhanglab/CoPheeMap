# CoPheeMap: A Machine-Learned Co-Regulation Map of 26,280 Phosphosites

## Table of Contents

- [Introduction](#introduction)
- [Usage: Google Colab Notebooks](#usage-google-colab-notebooks)
- [Usage: Running Locally](#usage-running-locally)
  - [Installation Requirements](#installation-requirements)
  - [Steps](#steps)
- [Citation](#citation)
- [License](#license)

---

## Introduction

Mass spectrometry-based phosphoproteomics offers a comprehensive view of protein phosphorylation, yet limited knowledge about the regulation and function of most phosphosites restricts the extraction of meaningful biological insights. **CoPheeMap** addresses this challenge by combining machine learning with phosphoproteomic data from 1,195 tumor specimens spanning 11 cancer types, creating a co-regulation network of **26,280 phosphosites**.

**Key Features:**

- **CoPheeMap** constructs a co-regulation map of phosphosites.
- **CoPheeKSA** predicts kinase-substrate associations, revealing associations between 9,399 phosphosites and 104 kinases (including under-studied kinases).
- Highlights biologically significant phosphosites and identifies potential therapeutic targets.

For detailed information, refer to our [bioRxiv preprint](https://doi.org/10.1101/2024.03.19.585786).

---

## Usage: Google Colab Notebooks

| Component | Description | Notebook |
|-----------|-------------|----------|
| **CoPheeMap** | Supervised learning model to construct a co-regulated phosphosite network | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/bzhanglab/CoPheeMap/blob/main/CoPheeMap.ipynb) |
| **CoPheeKSA** | Predict kinase-substrate associations using CoPheeMap | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/bzhanglab/CoPheeMap/blob/main/CoPheeKSA_XGBoost.ipynb) |
| **PSSM** | Generate PSSM matrices from gold-standard KSAs | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/bzhanglab/CoPheeMap/blob/main/PSSM.ipynb) |

---
## Usage: Running Locally

### Installation requirements

- Python 3.8 or later
- Required Python libraries: numpy, pandas, scikit-learn, matplotlib
- Jupyter Notebook (for running Colab notebooks locally)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/CoPheeMap.git
   cd CoPheeMap
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---


To run the notebooks locally:

1. Install Jupyter Notebook:
   ```bash
   pip install notebook
   ```
2. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Open the desired `.ipynb` file and execute the cells. Follow the instructions in each notebook to:
   - Construct the co-regulation map (CoPheeMap).
   - Predict kinase-substrate associations (CoPheeKSA).
   - Generate PSSM matrices.

---

## Citation

If you use CoPheeMap or CoPheeKSA in your research, please cite:

```bibtex
@article{jiang2024,
  title={Illuminating the Dark Cancer Phosphoproteome Through a Machine-Learned Co-Regulation Map of 26,280 Phosphosites},
  author={Jiang W, Jaehnig EJ, Liao Y, Yaron-Barir TM, Johnson JL, Cantley LC, Zhang B},
  journal={bioRxiv},
  year={2024},
  doi={10.1101/2024.03.19.585786}
}
```

---

## License

This repository is licensed under the MIT License. See the [LICENSE](https://github.com/bzhanglab/CoPheeMap/blob/main/LICENSE) file for details.
