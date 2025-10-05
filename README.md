
# Proposed 3D Reconstruction — **ComfyUI Workflow**

This repository provides the **exact ComfyUI workflow** used in our experiments, plus external weight links, THUMAN 3.0 find-tuned SV3D ([Google Drive](https://drive.google.com/file/d/1-SwdkAyppx0Jp8Z0ZT_CLF7cIYA_wWFN/view?usp=drive_link)).

## Contents
- `comfyui/workflows/Final.json` (SHA256: `98a7430d9e71f73f04a39d3a31fb99016fe29e181e3bb273aedbb04361bdcb54`)
- `env/` environment info (ComfyUI commit, custom nodes list)
- `weights/README.md` (Google Drive link + SHA256 placeholder)

## Pure python Implementation
- A modular Pytorch that replicates the ComfyUi graph with deterministic configs and CLI
  Code: https://drive.google.com/file/d/10f5jPRN_zg4mHtWIXOpPIz5_lwOzJamC/view?usp=drive_link

## Usage
1. Install **ComfyUI** and required custom nodes (pin exact commits in `env/`).
2. Copy `comfyui/workflows/Final.json` into your ComfyUI `workflows/` folder.
3. Download weights from Google Drive (see `weights/README.md`). Place them under `ComfyUI/models/checkpoints/` (or the path your nodes expect).
4. Launch ComfyUI and open `Final.json`.

## Licensing & Reproducibility
- We do **not** redistribute licensed datasets/weights in this repo; instead, we provide **links** and ask users to verify **SHA256** after download.
- For deterministic runs, record: **ComfyUI commit**, **custom-node commits**, **seed**, and **prompts**.

##  Citation
If you use this workflow, please cite the repository (see `CITATION.cff`).
