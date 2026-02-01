# Models Repository

This repository contains model weights for the SPAD for Vision project.

## Model Structure

Models are organized by type:
- `dinov3/` - DINOv3 model weights
- `flat_surface/` - Flat surface detection models
- `material_detection_head/` - Material detection head models
- `material_purity/` - Material purity detection models
- `spatiotemporal/` - Spatiotemporal detection models
- `yolov3/` - YOLOv3 model weights
- `yolov8/` - YOLOv8 model weights

## Note

Due to GitHub's file size limitations, the actual model files are hosted on Hugging Face Hub:
- Organization: `mvplus`
- Model repositories: `mvplus/dinov3`, `mvplus/flat_surface`, etc.

## Usage

Models can be downloaded from Hugging Face Hub using:
```python
from huggingface_hub import snapshot_download
snapshot_download(repo_id="mvplus/dinov3", repo_type="model")
```

Or via the Hugging Face CLI:
```bash
huggingface-cli download mvplus/dinov3
```
