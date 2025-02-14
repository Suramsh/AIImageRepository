# Image Denoising and Enhancement Techniques

## Overview
This repository contains the implementation of various image denoising and enhancement techniques for 12-bit RAW images. The goal of this project is to apply and compare methods such as AI-based denoising, median filtering, bilateral filtering, and edge enhancement techniques using a Laplacian filter. The output is a 24-bit RGB image, suitable for further processing and analysis.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Results](#results)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Features
- Implementation of AI-based denoising using U-net Neural Network model. From [here](https://github.com/JavierGurrola/RDUNet) 
- Application of median and bilateral filters for traditional denoising.
- Edge enhancement using Laplacian filters.
- Evaluation metrics including spatial signal-to-noise ratio and edge strength.
- Modular and organized code structure for easy understanding and contributions.

## Technologies Used
- Python
- OpenCV
- PyTorch
- NumPy
- Matplotlib (for visualization)

## Getting Started
To get a local copy of this project up and running, follow these steps:

1. **Clone the repository:**
   ```bash
   cd C:/type/path/here
   git clone https://github.com/gauravnirmalkumar/AIDenoisingAndEdgeEnhancement.git
   cd AIDenoisingAndEdgeEnhancement
   ```
2. **Set up a virtual environment:** (Recommended: [Anaconda](https://www.anaconda.com/))
   ```bash
   conda create --name myenv
   conda activate myenv
   ```
3. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
## Usage
To run the main script, use the following command:
   ```bash
   python main.py
   ```
### Input
The input for the program should be a 12-bit RAW image file located in the data/ directory.

### Output
The denoised output will be saved in the output/ directory in 24-bit RGB format.

### Pre-trained Model
You can find the pre-trained model [here](https://drive.google.com/drive/folders/1jF8YF-7SoVpc4y39_lFl25OBFVQmZAWJ) (model_color.pth). Download the model_color.pth file and place it in the model_color/ directory for use in the denoising process.

## Results
### Denoising Example
Below are some examples of the denoising results achieved with this project.

#### AI denoised image using [RDUNet](https://github.com/JavierGurrola/RDUNet):
![AI_denoised_24bit](https://github.com/user-attachments/assets/3a34ed64-3c89-4483-9d01-6aea6f8657ec)

#### Commonly Used Algorithms
###### Bilateral filter:
![bilateral_filtered](https://github.com/user-attachments/assets/418f06bc-b308-44db-9e3d-3f2f074a3998)

###### Gaussian filter (Implemented in Assignment 1):
![gaussian_filtered](https://github.com/user-attachments/assets/2282ab21-2753-4f7b-853a-d548009f07c8)

###### Median filter:
![median_filtered](https://github.com/user-attachments/assets/7c123fc1-935f-4cb5-b88c-bf85a4610ec3)

## License
This project is licensed under the MIT License.

## Citation (AI U-Net for Image Denoising)
```
@article{gurrola2021residual,
  title={A Residual Dense U-Net Neural Network for Image Denoising},
  author={Gurrola-Ramos, Javier and Dalmau, Oscar and Alarcón, Teresa E},
  journal={IEEE Access},
  volume={9},
  pages={31742--31754},
  year={2021},
  publisher={IEEE},
  doi={10.1109/ACCESS.2021.3061062}
}
```

## Acknowledgments

[OpenCV Documentation](https://opencv.org/)
[PyTorch Documentation](https://pytorch.org/)

Special thanks to the contributors, and anyone who has provided feedback on this project.

Thanks for taking your time to get to the end :D
