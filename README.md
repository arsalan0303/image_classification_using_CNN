# Cat vs Dog Image Classification

A beginner-friendly image classification project using **PyTorch** and a **Convolutional Neural Network (CNN)** to distinguish between cat and dog images.

## Project overview

This notebook demonstrates:
- Image preprocessing and normalization
- Data augmentation for training images
- Loading images with `torchvision.datasets.ImageFolder`
- Creating DataLoaders
- Building a CNN with convolution, pooling and fully connected layers
- Training with Cross Entropy Loss and the Adam optimizer
- Validation accuracy
- Saving and loading the trained model
- Predicting a single image
- Final test accuracy, confusion matrix and classification report

## Dataset structure

The notebook uses the folder names from the original code:

```text
project-folder/
├── data1/
│   ├── training_set/
│   │   ├── cats/
│   │   └── dogs/
│   ├── validation_set/
│   │   ├── cats/
│   │   └── dogs/
│   └── test_set/
│       ├── cats/
│       └── dogs/
└── Image_classification.ipynb
```

Each split must contain `cats` and `dogs` folders. The notebook reads the dataset from `data1/`.

**Dataset note:** The image dataset is not included in this repository. Add it locally and check its license before redistribution.

## Requirements

- Python 3.9 or later
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- Pillow
- Jupyter Notebook

Install the libraries:

```bash
pip install -r requirements.txt
```

## Run the project

1. Clone or download this repository.
2. Put the dataset in the `data1/` folder using the structure shown above.
3. Install the requirements.
4. Open `Image_classification_with_markdown.ipynb` in Jupyter Notebook or VS Code.
5. Run the notebook cells from top to bottom.

## Results

After training, the notebook reports validation accuracy. At the end, it evaluates the model on the test dataset and displays:
- Test accuracy
- Precision, recall and F1-score for each class
- Confusion matrix

**Results are not hard-coded in this README.** Run the notebook on your dataset and copy the actual metrics here.

Example format to complete after running:

| Metric | Your result |
|---|---:|
| Validation accuracy | Add your measured value |
| Test accuracy | Add your measured value |

## Model

The CNN contains two convolutional layers with ReLU activation and max-pooling, followed by flattening and fully connected layers. The output layer predicts one of two classes.

## Future improvements

- Use separate non-augmented transforms for validation and test data.
- Add training and validation loss plots.
- Compare the baseline CNN with a pretrained model such as ResNet.
- Tune the number of epochs, batch size and learning rate.

## License

Add a license appropriate for your project and confirm that the dataset license permits your intended use.
