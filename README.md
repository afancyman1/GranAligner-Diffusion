# GranAligner-Diffusion

This repository contains the official implementation of our AAAI 2026 submission:  
**GranAligner: Multi-Granular Scene-Object Consistency for Text-to-Image Synthesis**  
*(Submitted to AAAI 2026)*

We propose GranAligner, a novel diffusion framework that integrates linguistic cues to refine multi-granularity conceptual consistency through reward-based optimization. 

This repository includes an anonymized and functional subset of our full implementation, sufficient for reproducing our core experimental results. Some non-essential engineering details are omitted for confidentiality purposes during peer review.


## Getting Started

Clone this repository and set up the environment using the provided Conda configuration:

### 1. Clone the repository and create the Conda environment
```bash
git clone https://github.com/afancyman1/GranAligner-Diffusion
cd GranAligner-Diffusion
conda env create -f environment.yaml
conda activate gran_aligner_diffusion
```

### 2. Download required model weights
```bash
cd weights
wget "https://huggingface.co/spaces/xinyu1205/Tag2Text/resolve/main/tag2text_swin_14m.pth" -O tag2text_swin_14m.pth
```

### 3. Download Stable Diffusion checkpoint
Download the official Stable Diffusion v1.5 checkpoint (model.ckpt) and place it under models/ldm/stable-diffusion-v1/.

## Overview
All experiments can be run via the provided `demo.ipynb` notebook.

## Acknowledgements

[fenneishi/Tag2Text](https://github.com/fenneishi/Tag2Text)
[lm-sys](https://github.com/lm-sys)/**[FastChat](https://github.com/lm-sys/FastChat)
