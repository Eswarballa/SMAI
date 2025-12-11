| **Model Tried**                             | **Details**                                | **Score / MAE**                                      |
| ------------------------------------------- | ------------------------------------------ | ---------------------------------------------------- |
| Basic CNN                                   | 2 Conv layers, MaxPool, ReLU               | **8.65**                                             |
| Deeper CNN                                  | More Conv layers                           | *Slight improvement*                                 |
| VGG16 / VGG19                               | Pretrained, Transfer Learning              | *Moderate improvement*                               |
| Inception / Xception                        | Pretrained models tested                   | *Moderate improvement*                               |
| Vision Transformer (ViT)                    | 10 → 20 → 30 epochs                        | Performance improved, then plateaued *(overfitting)* |
| **DeiT (Data-Efficient Image Transformer)** | 15 epochs                                  | **Best single-model performance**                    |
| DeiT + Augmentation                         | 25 epochs                                  | Better than basic DeiT                               |
| **Model Averaging (Ensemble)**              | Combined DeiT-15, DeiT-25, DeiT-20 outputs | **Final best score**                                 |
