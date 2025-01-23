# SkinLesionClassification-ResNet18

## Project Goal

This project aims to develop an automated skin lesion classification system using deep learning, with the goal of achieving high accuracy in classifying various types of skin lesions. Early and accurate diagnosis of skin cancer significantly increases the chances of successful treatment and recovery. This project focuses on building a reliable and efficient deep learning model to assist in the classification of skin lesions, potentially aiding healthcare professionals in making timely and accurate diagnoses. 

## Dataset

The HAM10000 ("Human Against Machine with 10000 training images") dataset, comprising 10,015 dermatoscopic images, is used for this project. These images are categorized into seven distinct classes of skin cancer lesions, providing a diverse and comprehensive dataset for training and evaluating the deep learning model. 

* Data Acquisition
    * The HAM10000 dataset was accessed from the Harvard Dataverse. 
* Data Preprocessing
    * The dataset was preprocessed to ensure data quality and consistency. This involved steps such as image resizing, normalization, and data augmentation to enhance the dataset's size and variability. 
* Data Structure and Attributes
    * The dataset includes images in JPG format with corresponding labels indicating the type of skin lesion. 
    * Additional metadata, such as patient demographics and lesion characteristics, may be included in the dataset. 
* Dataset Composition and Classes
    * The dataset contains 10,015 images. 
    * The images are classified into seven distinct classes of skin cancer lesions. 

## Methodology

* Model Selection
    * A pre-trained ResNet-18 model was selected for its proven effectiveness in image classification tasks. 
    * Transfer learning was employed to leverage the knowledge learned from a large-scale dataset (ImageNet) and fine-tune it for skin lesion classification. 
* Model Training
    * The ResNet-18 model was fine-tuned using a custom training loop with appropriate optimizers and loss functions. 
    * The model was trained for 50 epochs to optimize its performance on the skin lesion classification task. 
* Model Evaluation
    * The model's performance was evaluated using metrics such as accuracy, loss, and confusion matrices.
    * Grad-CAM analysis was utilized to provide visual explanations of the model's predictions, highlighting the regions of the image that influenced the classification decision.

## Results

* The fine-tuned ResNet-18 model achieved an overall accuracy of 83% on the HAM10000 dataset.
* Class-specific accuracies varied, with some classes achieving higher accuracy than others, indicating potential areas for improvement.
* Grad-CAM analysis provided insights into the model's decision-making process, highlighting the regions of the image that were most influential in the classification.

## Usage

To run this project, follow these steps:

1.  Clone the repository.
2.  Navigate to the project directory.
3.  Create a virtual environment (recommended).
4.  Install the required dependencies.
5.  Download the HAM10000 dataset.
6.  Run the preprocessing script to prepare the data.
7.  Run the training script to train the model.
8.  Run the evaluation script to evaluate the model's performance.

## Conclusion

This project successfully demonstrated the effectiveness of deep learning in classifying skin lesions. The fine-tuned ResNet-18 model achieved a high accuracy on the HAM10000 dataset, showing promise for future applications in medical imaging and diagnostics.

## Future Work

* Explore other deep learning architectures and compare their performance.
* Implement more advanced data augmentation techniques to further improve model generalization.
* Develop a web application or API to deploy the model for real-world use.