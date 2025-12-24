# Task [X]: [Task Name]

**Student:** Hümbətova Nəzrin  
**ID:** S213  
**Seed:** 20240113

## Presentation
[View Presentation Slides](https://docs.google.com/presentation/d/1pdCCM7jT3JeaF3-0h98xG6cHjXcsgfHn/edit?pli=1&slide=id.p1#slide=id.p1)

## Dataset
- **Name:** Potato Disease Classification
- **Classes:** 3
- **Training samples:** 1721
- **Test samples:** 431

## Model Architecture
- **Type:** ResNet18
- **Convolutional layers:** 17
- **Fully connected layers:** 1
- **Total parameters:** 11,177,539

## Training Comparison

### Version 1
- **Learning rate:** 0.0001
- **Batch size:** 32
- **Optimizer:** Adam
- **Test accuracy:** 89.56%

### Version 2
- **Learning rate:** 0.0001
- **Batch size:** 64
- **Optimizer:** Adam
- **Test accuracy:** 84.69%

### Best Result
- **Best version:** Version 1
- **Final test accuracy:** 89.56%
- **Target accuracy:** 85.00%
- **Status:** ✓ Achieved

## Analysis
- **Best performing class:** Potato___Healthy
- **Worst performing class:** Potato___Early_blight
- **Key observations:** Version 1 (batch size 32) achieved higher accuracy (89.56%) compared to Version 2 (84.69%), suggesting smaller batches improved generalization on this specific dataset size. The model successfully utilized transfer learning features to classify diseases despite the added Gaussian blur and color jitter augmentation.

## Files
- `notebook.ipynb`: Complete implementation with both training runs
- `results/training_comparison.png`: Comparison of Version 1 vs Version 2
- `results/confusion_matrix.png`: Confusion matrix from best model
- `results/predictions.png`: Sample predictions
