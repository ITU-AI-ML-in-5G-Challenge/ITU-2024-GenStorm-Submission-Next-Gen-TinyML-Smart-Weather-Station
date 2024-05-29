# ITU-2024-GenStorm-Submission-Next-Gen-TinyML-Smart-Weather-Station

This repository contains model code and technical report by team GenStorm for the Next-Gen tinyML Smart Weather Station Challenge 2024 by ITU.

## Repository Contents

1. **arduino_code_GenStorm Directory**
    - Contains our model Arduino code implementation and its library deployed from the Edge Impulse platform.

2. **model Directory**
    - Includes all our model files in `.tflite`, `.keras`, and `.h5` formats.

3. **Next-Gen-TinyML-Smart-Weather-Station-GenStorm-Report.pdf**
    - Our comprehensive project report.

4. **Next-Gen-TinyML-Smart-Weather-Station-GenStorm-Demo-Video.mp4**
    - A demo video showcasing our weather station in action.

5. **Dataset**
    - The dataset used for this work can be downloaded from [Dataset Link](https://drive.google.com/drive/folders/1cb6_lLHbga0Q5yfVWKS1eW84Z06jm6tx).

6. **Next-Gen-TinyML-Smart-Weather-Station-GenStrom-PresentationSlides.ppt**
    - Our presentation slides can be found here.


## Project Overview

In the face of escalating climate challenges, precise weather monitoring is crucial for community resilience and adaptation. The "Next-Gen tinyML Smart Weather Station Challenge 2024" is a beacon for innovation in environmental monitoring. Team GenStorm has designed an intelligent model for classifying rainfall intensity using the Edge Impulse platform, deployed as an Arduino library. Our weather station also records pressure and temperature, optimized for power efficiency to ensure longevity and effectiveness.

## Problem Statement

Accurate weather monitoring is vital for agricultural productivity and sustainability. Existing weather stations are often expensive, complex, and prone to failure, especially in remote or resource-limited settings. This project aims to create a low-cost, low-power, reliable, and accurate weather station that can measure various weather conditions, focusing on rain and wind intensities, without mechanical moving parts. The intended application is in agricultural environments, providing farmers with real-time local weather data to make informed crop planting and management decisions.

## Data Collection and Processing

The dataset, collected by AI4Africa in September 2022 in Kogi State, Nigeria, includes audio recordings of rainfall captured using a mobile phone. The recordings, categorized into five rainfall intensity classes, are used to train our model. The preprocessing involves Mel-filterbank energy (MFE) feature extraction, crucial for classifying the rainfall intensities.

## Model Design and Training

Our neural network, based on a 1D convolutional neural network architecture, is optimized for classifying rainfall intensity from audio data. Trained over 300 cycles with a learning rate of 0.005, the model achieves a test accuracy of 97.47%. Post-quantization, the model size is reduced to 10 KB, making it highly efficient for deployment on low-power hardware.

## Deployment

The model is deployed as an Arduino library on the Arduino Nano 33 BLE Sense, enabling real-time rain monitoring. The board’s built-in sensors and processing capabilities, along with power optimization measures, ensure efficient operation and extended runtime.

## Authors

- Fortunatus Aaabangbio. Wulnye: [fortunatuswulnye@outlook.com](mailto:fortunatuswulnye@outlook.com)
- Dennis Agyemanh Nana Gookyi: [dennisgookyi@gmail.com](mailto:dennisgookyi@gmail.com)
- Roger Kwao Ahiadormey: [rogerkwao@gmail.com](mailto:rogerkwao@gmail.com)

## Acknowledgments

We thank AI4Africa for providing the dataset and the ITU for organizing the Next-Gen tinyML Smart Weather Station Challenge 2024, fostering innovation in environmental monitoring.

---

For detailed information on the project, refer to the `Next-Gen-TinyML-Smart-Weather-Station-GenStorm-Report.pdf`. The demo video `Next-Gen-TinyML-Smart-Weather-Station-GenStorm-Demo-Video.mp4` provides a visual overview of the project implementation.

---
