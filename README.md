# Image Segmentation for the Detection of Hard Exudates in Diabetic Retinopathy 👁️🩺
## Project description
* Deep learning–based image segmentation for hard exudate detection in Diabetic Retinopathy, addressing a highly imbalanced medical imaging problem using retinal fundus images from the **IDRiD dataset**.
* **Comprehensive preprocessing pipeline** including CLAHE contrast enhancement, patch extraction (512×512, overlapping stride), and data augmentation (flips, brightness and hue variations) to improve lesion visibility and model generalization.
* Evaluation and comparison of multiple segmentation architectures: **modified UNet, Attention UNet, DeepLabV3, and Swin UNETR**, implemented in PyTorch and trained on GPU.
* **Systematic loss function analysis: Weighted BCE, Focal Loss, Tversky Loss**, identifying **Weighted BCE** as the most effective for maximizing lesion recall in highly imbalanced settings.
* Introduction of a novel **negative-mask strategy** to penalize false positives in regions occupied by other retinal lesions, significantly improving precision and Dice score for UNet and Attention UNet.
* Best overall performance achieved by Swin UNETR, reaching **Dice = 0.693 and AUC-PR = 0.738**, demonstrating the advantage of transformer-based architectures in capturing both local and global retinal features. 
