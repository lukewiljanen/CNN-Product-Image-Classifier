# CNN-Product-Image-Classifier
Comparing four models for e-commerce product image classification on Kaggle’s Fashion Product Images: a fully connected network, a CNN from scratch, a convolutional autoencoder, and a fine-tuned ResNet50. Built with TensorFlow/Keras for CPSC 393 (Fall 2026).

**Team:** Luke Wiljanen, Ashlee Nguyen, Auggie Pirazzi

## Getting started
```bash
pip install -r requirements.txt
jupyter notebook product_image_classifier.ipynb
```
The notebook downloads the dataset the first time it runs with `kagglehub` (cached after that). The code follows the style of the [CPSC 393 class labs](https://github.com/rhamzaali/CPSC393-MachineLearning/tree/main/class_labs), and several helper functions are adapted from them.

## Layout
| Path | What it is |
|---|---|
| `product_image_classifier.ipynb` | The whole project, one section per part |
| `splits/` | Train/val/test split CSVs; built once, committed, shared by every model |
| `figures/` | Saved figures for slides and the report |
| `models/` | Saved trained models (git-ignored) |

## Working together
- Each person works on their own branch and opens a pull request into `main`.
- Only edit your own section of the notebook.
- Clear outputs before committing (*Kernel → Restart & Clear Output*) to avoid merge conflicts.
- Don't re-split: once `splits/` is committed, the notebook loads it.
