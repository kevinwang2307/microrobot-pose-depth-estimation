# Microrobot Pose & Depth Estimation with Deep Learning

PyTorch models for microscopy images to predict:
- **Pose**: 40-class pitch/roll classification  
- **Depth**: regression

This repo contains the project **notebook + report**. The dataset and trained weights are **not included**.

## Results (from report)
- **Pose**: 0.88 test accuracy (F1 ≈ 0.88)
- **Depth**: RMSE 0.137, R² 0.983

## Approach (high level)
- Benchmarked custom CNN variants (V1/V2/V3) against **ResNet18**
- Used validation-based model selection (**early stopping**)
- Performed error analysis on failure cases where similar poses created depth ambiguity

## Repository contents
- `notebooks/microrobot_pose_depth.ipynb` — training, evaluation, and analysis
- `report.pdf` — full write-up and results
- `saved_models/` — local checkpoints (gitignored)

## Setup
```bash
pip install -r requirements.txt
