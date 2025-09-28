﻿# dl-pro-jects

Collection of deep learning playground notebooks.

- `notebooks/multi_layer_perceptron.ipynb`: NumPy-only multi-layer perceptron with backprop, training loop, and visualisations. Uses `data/mock_classification.csv` as a ready-made multi-class dataset.
- `notebooks/pytorch_mle_playbook.ipynb`: PyTorch tips for senior MLEs covering latency tuning, memory patterns, quantization, pruning, and exporting to ONNX / TensorRT / TFLite.
- `notebooks/gnn_node_clustering.ipynb`: A prototype for unsupervised cohort detection using a GraphSAGE Graph Neural Network (GNN) to find clusters in a graph.

## Environment

Create the shared environment:

`bash
conda env create -f environment.yml
conda activate dl-projects
`
 
> **Note**
> If you get a `conda: command not found` error, you need to initialize your shell.
> 1. Open the **Miniconda Prompt** from your Windows Start Menu.
> 2. Run `conda init --all`.
> 3. Close the prompt and open a new terminal. The `conda` command should now work.
`

Launch Jupyter once the environment is active:

`bash
jupyter notebook
`

Optional extras:
- Install GPU-enabled PyTorch or Torch-TensorRT if your hardware supports it.
- Swap in your own datasets by replacing files under data/.
