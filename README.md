# flower-recognition-agritech

This project develops an advanced automatic flower recognition prototype to optimize agricultural monitoring and enhance real-time plant health assessments. Manual crop evaluation is highly inefficient, labor-intensive, and prone to human error; this solution addresses these bottlenecks by implementing a robust deep learning image classifier engineered to operate within variable environmental conditions.

The system incorporates a highly optimized transfer learning and data augmentation workflow using PyTorch and the `timm` library:
* **Targeted Architectural Selection:** Deploying a state-of-the-art `convnext_tiny.fb_in22k_ft_in1k` backbone to ensure rapid training convergence and powerful feature feature extraction despite hardware and computation constraints.
* **Aggressive Regularization & Augmentation:** Implementing a multi-stage transformation matrix including localized `GaussianBlur`, `ColorJitter`, and structural flips to prevent overfitting on smaller sample fragments while preserving key macro morphological features.
* **Precision Performance Auditing:** Establishing a tailored binary tracking logic focused strictly on maximizing the Macro F1-Score to counteract class distribution imbalances and maintain evaluation stability across target datasets.

The final execution achieves an exceptional macro F1-Score of 0.9944 and a test accuracy of 99.45% on the test subset, establishing an industrial-grade visual baseline for edge-AI processing in modern sustainable digital agriculture.

To see more, extended explanation in the project.
