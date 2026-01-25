# Evaluation

## 1) Semantic parsing metrics
- mIoU, F1, Precision, Recall, Accuracy

You can run evaluation by exporting generated images and semantic maps, then
computing parsing metrics with your favorite segmentation evaluator.

## 2) Appearance / consistency
- PSNR, SSIM, LPIPS, CLIP-Score, FID, DINO, CLIP-IQA
- CLIP-based metrics (e.g., CLIP-MF: average pairwise similarity across façades of the same building)

> Tip: report both quality (IQA/perceptual) and consistency; pure consistency can be trivially high if all façades collapse to the same texture.
