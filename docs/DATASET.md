
# Dataset Documentation

## 1. Dataset Overview

The project uses a facial image dataset to classify faces into four categories:

- Heart
- Oval
- Round
- Square

## 2. Dataset Structure

The dataset is divided into two folders:

- `training2` – Training images
- `testing2` – Testing images

Each folder contains four class-specific subfolders.

## 3. Dataset Distribution

| Face Shape | Training Images | Testing Images | Total |
|---|---:|---:|---:|
| Heart | 4 | 2 | 6 |
| Oval | 4 | 2 | 6 |
| Round | 4 | 2 | 6 |
| Square | 4 | 2 | 6 |
| **Total** | **16** | **8** | **24** |

## 4. Dataset Usage

Training images are used during model development, while testing images are reserved for evaluating the trained model.

## 5. Limitations

The current dataset is small. Therefore, model evaluation results should be interpreted cautiously. A larger and more diverse dataset would be required for reliable generalisation.
