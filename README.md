# srdiff

This project is an implementation of super-resolution using diffusion models (SRDiff).

## Dataset

The project uses the **DIV2K High-Resolution Images** dataset from Kaggle:
[Kaggle DIV2K Dataset](https://www.kaggle.com/datasets/soumikrakshit/div2k-high-resolution-images)

## Project Structure

- srdiff (5).ipynb: Original project notebook.
- srdiff (11).ipynb: Updated notebook containing robust evaluation metrics (PSNR, SSIM, LPIPS) to measure super-resolution performance against deterministic baselines like RRDB. Includes representative visual results while maintaining a compact size for GitHub rendering.
- srdiff_pretrained_div2k/: Directory containing pre-trained model weights.

## Evaluation & Results

We employ rigorous metrics to evaluate the performance of our diffusion-based super-resolution models on the DIV2K dataset:
- **PSNR** (Peak Signal-to-Noise Ratio): Evaluates pixel-level fidelity.
- **SSIM** (Structural Similarity Index): Measures structural resemblance to the ground truth.
- **LPIPS** (Learned Perceptual Image Patch Similarity): Captures human-perceived visual quality and perceptual distance.

The srdiff (11).ipynb notebook tracks these evaluation metrics across stochastic diffusion ensembles and compares them against our deterministic baselines to achieve state-of-the-art super-resolution generation.
