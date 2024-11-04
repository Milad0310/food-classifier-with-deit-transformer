
<p align="center">
  <img src="results\deit-original-results.png" alt="Image 1" width="45%">
  <img src="results\model_shape.png" alt="Image 2" width="45%">
  <img src="results\result.png"" alt="Image 3" width="45%">
</p>

## Project Description

This project demonstrates the use of the Data-efficient Image Transformer (DeiT) model for food image classification. The goal is to efficiently classify various types of food images, leveraging the power of transformer-based models for image recognition. By using DeiT, this project aims to achieve high accuracy with reduced data requirements, making it suitable for real-world applications like menu recognition or dietary analysis.

### Motivation and Problem Statement

The motivation for this project stems from the growing demand for efficient and accurate food recognition systems in the fields of dietary management, food delivery, and nutrition analysis. Traditional convolutional neural networks can be resource-intensive; DeiT offers an optimized alternative that requires less data while maintaining high accuracy. This project aims to simplify food recognition, making it accessible and practical for industries and users alike.

### Technologies Used

- **DeiT Transformer**: Chosen for its data efficiency and effectiveness in image classification tasks.
- **PyTorch**: For implementing and training the model, given its flexibility and robust community support.
- **Python**: Core language used for data processing, training, and evaluation.
- **Google Colab**: Utilized for leveraging free GPU resources to train and test the model.

## Installation and Setup

### Prerequisites

Before you start, ensure you have the following installed:

- Python (>=3.7)
- PyTorch (>=1.7)
- Additional Python libraries: `torchvision`, `numpy`, `pandas`, and `matplotlib`

### Step-by-Step Setup

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/food-classifier-with-deit-transformer.git
   cd food-classifier-with-deit-transformer
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Download and prepare the dataset by placing the food images in the `data/` folder.

4. Run the training script to start training:
   ```bash
   python food-train.py
   ```

5. After training, use the following command to test the model:
   ```bash
   python predict.py
   ```

## Project Structure

```
food-classifier-with-deit-transformer/
│
├── models/              # Directory for saving trained model weights
├── results/             # Folder to store results and output images
├── README.md            # Project documentation
├── requirements.txt     # Required Python libraries
└── LICENSE              # Project license
```

## How to Use the Project

1. **Training**: To train the model on your custom dataset, modify the data loading section in `food-train.py` and place your dataset in the `data/` directory.
2. **Inference**: Run `predict.py` to classify new food images..

## Challenges

One challenge encountered was optimizing DeiT for smaller datasets without overfitting. This was addressed by incorporating data augmentation techniques and regularization during training.

## Credits
- [DeiT Paper by Facebook AI Research](https://arxiv.org/abs/2012.12877)

## License

This project is licensed under the GPL-3.0 License. See the [LICENSE](LICENSE) file for more details.

## How to Contribute

Contributions are welcome! If you have ideas for improvement, please fork the repository and submit a pull request. For major changes, open an issue first to discuss what you would like to change. Make sure to update tests as appropriate.
