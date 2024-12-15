# AI-Driven NSFW Content Moderation: Model Benchmarking

## Overview
This project focuses on the comprehensive analysis and benchmarking of eight deep learning models for NSFW (Not Safe For Work) content detection. Using a standardized dataset and consistent preprocessing, the models were trained and evaluated to determine their performance across key metrics, such as accuracy, precision, recall, F1-score, and ROC-AUC. The results offer valuable insights into the most effective architectures for NSFW classification, providing a foundation for future research and application development.

## Key Features
- Comparative analysis of eight deep learning models for NSFW content detection:
  - CNN, VGG16, ResNet, MobileNetV2, InceptionV3, AlexNet, NasNet, and LeNet.
- Evaluation using consistent metrics across a shared dataset.
- Comprehensive performance comparison for accuracy, efficiency, and scalability.
- Data preprocessing pipeline for balanced and uniform input resolution.

## Performance Metrics
Below is a summary of the performance of the evaluated models:

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
- **Primary Source**:
  - [NudeNet Classifier Dataset v1](https://archive.org/details/NudeNet_classifier_dataset_v1): A diverse dataset including nude and safe categories.
- Dataset Preprocessing:
  - Resized all images to a uniform resolution of 255x255 pixels.
  - Balanced training data with 200,000 images per class.

## Repository Structure
The repository is organized as follows:
- **`Layer Diagram/`**: Contains architecture diagrams for the various models used.
- **`Metrics/`**: Performance metrics of fine-tuned models.
- **`Models/`**: Includes pre-trained and fine-tuned model files info. Due to it's large size it exceeded the LFS limit.
- **`DL Models.ipynb`**: Notebook for training and evaluating deep learning models.
- **`Preprocessing Data.ipynb`**: Notebook for data preprocessing and augmentation.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/rayeanpatric/nsfw-comparison_analysis.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Use the provided notebooks (`DL Models.ipynb` and `Preprocessing Data.ipynb`) to:
   - Train and fine-tune models.
   - Preprocess datasets for consistent evaluation.

<!--## Research Paper
For detailed insights, please refer to the accompanying research paper:
[NSFW Content Moderation: Benchmarking Deep Learning Models](link-to-your-paper)-->

## Author
[Rayean Patric](https://www.linkedin.com/in/rayeanpatric/)
[Bharath Kumar](https://www.linkedin.com/in/bharath-kumar-k-75219721b)

## Contributing
Contributions are welcome! Please submit a pull request or open an issue for suggestions.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
