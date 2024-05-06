[Part 1 Link](https://colab.research.google.com/drive/1MDpViOHPwFn36lf54Ag5UdWJBUIou2Jw?usp=sharing)

[Part 2 & 3 Link](https://colab.research.google.com/drive/1om9S95jWarTMnynoXbzfpFf1da2mXPYM?usp=sharing)

# Action Recognition with I3D Model

## Overview

This document outlines the process of using the Inflated 3D Convnet (I3D) model, hosted on TensorFlow Hub, to recognize actions in video data. The I3D model, introduced by Joao Carreira and Andrew Zisserman in their paper "Quo Vadis, Action Recognition? A New Model and the Kinetics Dataset", has been pretrained on the Kinetics-400 dataset, which includes 400 different action categories.

## Objective

The primary goal was to demonstrate how to utilize the I3D model to recognize activities in videos from the UCF101 dataset. This dataset is a widely recognized collection of action videos which are ideal for evaluating action recognition models.

## Process Overview

1. **Environment Setup**:
   - Necessary Python packages such as TensorFlow, TensorFlow Hub, OpenCV, and ImageIO were installed to facilitate video processing and model operations.

2. **Model Loading**:
   - The I3D model was loaded from TensorFlow Hub, which provides a pre-trained model that can classify video into 400 action categories based on the Kinetics dataset.

3. **Video Processing**:
   - A video from the UCF101 dataset was downloaded and processed to fit the input requirements of the I3D model. This included resizing frames, converting color channels, and normalizing pixel values.

4. **Action Prediction**:
   - The processed video was passed through the I3D model to predict the probabilities of different actions. The top five predicted actions were then displayed.

5. **Error Handling**:
   - Adjustments were made to the video processing steps to ensure compatibility with the model's input expectations and to resolve issues related to data types and array shapes.

## Challenges and Resolutions

- **Data Type Compatibility**:
  - Initially faced challenges with data types that the PIL library could not handle. Resolved by ensuring that video frames were correctly converted to a compatible format (`uint8`) and scaled appropriately before converting to GIF for visualization.

- **Model Input Requirements**:
  - Adjusted input processing to match the model’s expectations, specifically ensuring that frame dimensions and data types matched the required specifications of the I3D model.

## Conclusion

The use of the I3D model from TensorFlow Hub demonstrated effective action recognition within video data, showcasing the model's capability to classify complex video sequences into categorized actions. Adjustments and error handling were crucial in adapting the video data to meet the model’s requirements and in effectively interpreting the model's outputs.


---


# Multi-Modal Machine Learning Demonstrations

## Overview

This document outlines the processes and methodologies employed in using advanced machine learning models to recognize patterns and make predictions based on video, text, and audio data. This includes leveraging pre-trained models for action recognition in video, semantic analysis in text, and event detection in audio streams.

## Objective

The primary goals were to:
- Demonstrate action recognition in videos using the Inflated 3D Convnet (I3D) model.
- Perform semantic analysis of text using machine learning models to compare different texts and understand their semantic similarities.
- Recognize specific events in audio data using the YAMNet model.

## Process Overview

### Video Data Processing and Action Recognition

1. **Model Loading**: Loaded the I3D model from TensorFlow Hub, pre-trained on the Kinetics-400 dataset.
2. **Video Processing**: Processed videos from the UCF101 dataset to fit the input requirements of the I3D model.
3. **Action Prediction**: Analyzed processed videos to predict action categories and displayed the top predicted actions.

### Text Data Analysis

1. **Semantic Similarity**: Utilized advanced NLP models to analyze the semantic similarities between different pieces of text.
2. **Text Comparisons**: Compared literary works to understand thematic and stylistic elements.

### Audio Data Event Detection

1. **Model Loading**: Loaded the YAMNet model from TensorFlow Hub, capable of detecting 521 audio events.
2. **Audio Processing**: Processed audio clips to extract meaningful features for event detection.
3. **Event Prediction**: Classified audio segments into predefined categories based on detected events.

## Challenges and Resolutions

- **Video Processing**: Addressed compatibility issues with video data types and array shapes to align with the I3D model's input requirements.
- **Audio Data Handling**: Adjusted audio data processing to ensure compatibility with YAMNet's expectations, particularly with respect to data types and sampling rates.
- **Text Data Insights**: Tackled challenges in natural language processing to accurately compare and contrast different texts based on semantic content.

## Tools and Technologies Used

- **TensorFlow and TensorFlow Hub**: For loading and utilizing pre-trained models.
- **OpenCV and ImageIO**: For video processing and GIF creation.
- **Natural Language Processing Libraries**: For text analysis and semantic comparison.

## Conclusion

The use of advanced machine learning models demonstrated effective recognition and analysis capabilities across different data modalities. Each modality presented unique challenges, particularly in data preprocessing and model compatibility. The project highlighted the robustness of pre-trained models in handling real-world data and generating actionable insights.


