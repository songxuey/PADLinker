# PADLinker
## Overview

TopoBond-DynAnchor is a conditional autoregressive graph model for PROTAC linker generation. Given two molecular fragments and their attachment sites, it combines a Graph Transformer, atom and directed bond graph encoders, and a dynamic anchor mechanism to generate a connecting linker.

The model constructs linkers through five graph-building actions using a breadth-first frontier strategy. Predicted generation progress guides the dynamic anchor mechanism without requiring the target linker length as an input. Training supports ZINC pretraining, continued training on GEOM, and PROTAC fine-tuning.

## Installation

Install the required Python packages:

```bash
python -m pip install torch rdkit numpy tqdm
```

For GPU support, install a PyTorch build compatible with your CUDA environment.
