# American Sign Language Recognition using CNNs

A computer vision and deep learning project that uses a Convolutional Neural Network (CNN) to recognise American Sign Language (ASL) hand gestures from image data.

The project explores how CNN-based image classification can support accessibility-focused translation systems by identifying ASL gestures and analysing the practical challenges involved in real-world deployment.

## Overview

American Sign Language is a critical communication method for deaf and hearing-impaired individuals, but communication barriers often arise when non-signers are unable to understand ASL.

This project investigates whether computer vision and deep learning can be used to classify ASL hand gestures from images. The system was developed as a prototype CNN-based recognition pipeline, with emphasis on dataset preparation, preprocessing, model training, evaluation, and analysis of limitations.

## Key Features

- CNN-based ASL gesture classification
- Image dataset preparation and cleaning
- Image resizing and preprocessing pipeline
- Train-validation workflow for model evaluation
- Class-wise performance analysis
- Accuracy and loss behaviour analysis
- Identification of overfitting and dataset imbalance issues
- Discussion of real-world generalisation constraints

## Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- pandas
- Matplotlib
- Computer Vision
- Convolutional Neural Networks

## Methodology

The project followed an end-to-end machine learning workflow:

1. **Data Collection**
   - ASL gesture images were collected using a Python-based workflow.
   - Low-quality or unsuitable images were removed during dataset cleaning.

2. **Data Preprocessing**
   - Images were resized into a consistent format.
   - Image data was converted into numerical arrays suitable for CNN input.
   - Class labels were assigned for supervised learning.

3. **Model Development**
   - A CNN architecture was designed for multi-class image classification.
   - The model used convolutional layers for feature extraction, pooling layers for dimensionality reduction, and fully connected layers for final classification.

4. **Training and Validation**
   - The dataset was split into training and validation sets.
   - The model was trained to recognise visual patterns in ASL gesture images.
   - Performance was evaluated using accuracy, loss trends, and class-wise results.

5. **Evaluation**
   - The model’s predictions were analysed across different gesture classes.
   - Performance limitations were studied, including class imbalance, overfitting, lighting variation, gesture similarity, and lack of dataset diversity.

## Results and Analysis

The CNN was able to learn meaningful visual features from the training data, but the evaluation showed that strong validation performance did not always translate into reliable real-world generalisation.

Key observations:

- Some classes performed strongly under controlled conditions.
- Certain gestures were harder to classify due to visual similarity.
- Dataset imbalance affected recognition quality for underrepresented classes.
- Overfitting was observed where the model memorised training patterns instead of learning sufficiently general features.
- Lighting, hand orientation, background variation, and signing style remain major challenges for real-world deployment.

## Limitations

This project is a prototype and does not represent a fully deployable ASL translation system.

Current limitations include:

- Limited dataset diversity
- Class imbalance across gesture categories
- Controlled image conditions
- No real-time video recognition
- No facial expression or body posture interpretation
- Limited vocabulary scope
- Potential overfitting on visually consistent training samples

## Future Improvements

Potential improvements include:

- Expanding the dataset with more diverse signers, lighting conditions, and backgrounds
- Applying data augmentation such as rotation, zooming, brightness shifts, and flipping
- Balancing underrepresented gesture classes
- Adding dropout and regularisation to reduce overfitting
- Tuning hyperparameters such as learning rate, batch size, and training epochs
- Extending the model to real-time webcam-based recognition
- Incorporating facial expressions and body posture for more complete ASL interpretation

## Project Significance

This project demonstrates the potential of computer vision and CNNs in accessibility-focused applications. While the model is not yet suitable for full real-world ASL translation, it establishes a strong foundation for gesture recognition and highlights the technical challenges involved in building inclusive AI systems.

## Author

**Suryansh Sharma**  
Computer Science Undergraduate  
BITS Pilani Dubai
