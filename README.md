Task 13: Potato Disease Classification

Student: Hümbətova Nəzrin
ID: S213
Seed: 20240113

Presentation

[View Presentation Slides](https://drive.google.com/your-link-here)


Dataset

Name: PlantVillage (Potato Subset)

Classes: 3

Training samples: 1721

Test samples: 431

Model Architecture

Type: ResNet18 (Transfer Learning)

Convolutional layers: 17

Fully connected layers: 1

Total parameters: ~11.7 Million

Training Comparison
Version 1

Learning rate: 0.0001

Batch size: 32

Optimizer: Adam

Test accuracy: 89.56%

Version 2

Learning rate: 0.0001

Batch size: 64

Optimizer: Adam

Test accuracy: 84.69%

Best Result

Best version: Version 1

Final test accuracy: 89.56%

Target accuracy: 85.00%

Status: ✓ Achieved

Analysis

Best performing class: Potato___Healthy

Worst performing class: Potato___Early_blight

Key observations: Version 1 (Batch Size 32) consistently outperformed Version 2 (Batch Size 64), reaching nearly 90% accuracy. The model successfully learned to classify the diseases despite the added Gaussian Blur and Color Jitter noise transformations.

Files

notebook.ipynb: Complete implementation with both training runs

results/training_comparison.png: Comparison of Version 1 vs Version 2

results/confusion_matrix.png: Confusion matrix from best model

results/predictions.png: Sample predictions
