# Concise Tutorial on Deep Learning

This repository contains a concise Chinese tutorial for deep learning, including
course slides and executable Jupyter notebooks.

## Contents

- `代码/`: example notebooks and supporting Python code
- `课件/`: course slides
- `requirements.txt`: Python dependencies used by the notebooks

## Topics

The tutorial covers:

- deep learning basics
- PyTorch fundamentals
- neural networks and fully connected models
- convolutional neural networks
- sequence models
- generative models
- large models and Transformer-based methods

## Data And Model Files

Large datasets, trained weights, generated outputs, and local runtime caches are
not tracked in this repository. If a notebook requires data or a pretrained
model, download or generate it locally according to the notebook instructions.

The `.gitignore` file excludes common local artifacts such as `data/`,
`.ipynb_checkpoints/`, `__pycache__/`, model weights, and training outputs.

## Usage

Install the dependencies first:

```bash
pip install -r requirements.txt
```

Then open the notebooks under `代码/` with Jupyter Notebook, JupyterLab, or VS
Code.
