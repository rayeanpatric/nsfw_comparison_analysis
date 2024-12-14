# Comparison Analysis of NSFW Content Moderation

## Overview
This project presents an AI-driven framework for detecting and moderating NSFW (Not Safe For Work) content, particularly focused on video uploads. By leveraging state-of-the-art deep learning models, the system performs frame-by-frame analysis to identify NSFW content and offers proactive options for handling explicit material. This approach enhances real-time moderation, ensuring user safety and regulatory compliance on social media platforms.

## Key Features
- Real-time NSFW content detection during video uploads.
- Efficient frame-by-frame analysis using **EfficientNet** and other deep learning models.
- User-guided options for managing detected content:
  - Labeling the video as 18+.
  - Censoring explicit content using Gaussian blur.
  - Canceling the upload.
- Automatic cleanup of temporary files to optimize server resources.
- Scalable and ethical AI-driven moderation for large platforms.

## Performance Metrics
The project involves a comparative analysis of various deep learning models. Below is a summary of their performance:

| **Model**       | **Accuracy** | **Precision** | **Recall** | **F1-Score** | **ROC-AUC** |
|------------------|-------------|---------------|------------|--------------|-------------|
| CNN              | 0.8200      | 0.8007        | 0.8622     | 0.8303       | 0.8956      |
| VGG16            | 0.8937      | 0.8749        | 0.9240     | 0.8988       | 0.9590      |
| ResNet           | 0.6475      | 0.6078        | 0.8738     | 0.7169       | 0.7589      |
| MobileNetV2      | 0.8816      | 0.8448        | 0.9410     | 0.8903       | 0.9615      |
| InceptionV3      | 0.9506      | 0.9269        | 0.9805     | 0.9530       | 0.9907      |
| AlexNet          | 0.8604      | 0.8521        | 0.8793     | 0.8655       | 0.9351      |
| NasNet           | 0.8281      | 0.7901        | 0.9035     | 0.8430       | 0.9200      |
| LeNet            | 0.7677      | 0.7231        | 0.8835     | 0.7953       | 0.8484      |

## Dataset
- **Primary Sources**:
  - [NudeNet Classifier Dataset v1](https://archive.org/details/NudeNet_classifier_dataset_v1): A diverse dataset including nude and safe categories.
  - E. Bazarov's dataset (Over 1.3 million NSFW images across 159 categories).
- Dataset Preprocessing:
  - Resized to a uniform resolution of 255x255 pixels.
  - Balanced training data with 200,000 images per class.

## Repository Structure
The repository is organized as follows:
- **`Layer Diagram/`**: Contains architecture diagrams for the various models used.
- **`Metrics/`**: Performance metrics of fine-tuned models.
- **`Models/`**: Includes pre-trained and fine-tuned model files.
- **`DL Models.ipynb`**: Notebook for training and evaluating deep learning models.
- **`Preprocessing Data.ipynb`**: Notebook for data preprocessing and augmentation.
- **`.gitattributes` and `.gitignore`**: Configuration files for managing repository metadata.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/nsfw-content-moderation.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Use the provided notebooks (`DL Models.ipynb` and `Preprocessing Data.ipynb`) to train models or preprocess datasets.

## Research Paper
For detailed insights, please refer to the accompanying research paper:
[NSFW Content Moderation: Benchmarking Deep Learning Models](link-to-your-paper)

## Contributing
Contributions are welcome! Please submit a pull request or open an issue for suggestions.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
