# Automatic Number Plate Recognition (ANPR)

This project uses computer vision techniques to detect and recognize vehicle number plates in images and videos. It leverages OpenCV for plate detection and EasyOCR for extracting text from detected plates, making it suitable for applications in traffic monitoring, automated parking systems, and law enforcement.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Project Structure](#project-structure)
- [Contributing](#contributing)

## Introduction

Automatic Number Plate Recognition (ANPR) is a technology that uses optical character recognition on images to read vehicle registration plates. This project focuses on detecting plates from images or video feeds, extracting the text, and displaying it in a readable format.

## Features

- Detect number plates in images and video files
- Real-time number plate detection using a webcam feed
- OCR-based text extraction for license plates

### Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

### Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/kalpesh-patel-20/ANPR-System.git
   cd ANPR-System
   ```

2. **Create a Virtual Environment** (recommended)

   ```bash
   python -m venv myenv
   myenv\Scripts\activate  # On Windows
   source myenv/bin/activate  # On macOS/Linux
   ```

3. **Install Dependencies**

   Use the `requirements.txt` file to install the necessary dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. **Download Haar Cascade File**

   Download the `haarcascade_russian_plate_number.xml` file from the [OpenCV GitHub repository](https://github.com/opencv/opencv/tree/master/data/haarcascades) and place it in a `model` directory.

   ```bash
   mkdir model
   # Move haarcascade_russian_plate_number.xml into the model directory
   ```

## Project Structure

```
ANPR-System/
├── model/
│   └── haarcascade_russian_plate_number.xml   # Haar Cascade file for plate detection
├── ocr-notebook/
│   └── easy_OCR_demo.ipynb
├── plates/
│   └── scanned_img_0.jpg   
├── number_plate.py                            # Main script for detection
├── requirements.txt                           # Required dependencies
└── README.md                                  # Project documentation
```

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a Pull Request.

