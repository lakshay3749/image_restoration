# Image Restoration for Surveillance Camera Systems

## Overview

This mini project focuses on restoring noisy surveillance images using classical image processing techniques.
In real CCTV systems, images captured in low light, fog, rain, or dusty environments often contain noise, which reduces visibility and affects identification accuracy.

The goal of this project is to simulate common noise conditions and restore image quality using spatial filtering methods.

---

## Objectives

* Understand real-world image noise in surveillance systems
* Simulate Gaussian and Salt & Pepper noise
* Apply image restoration filters
* Evaluate restoration quality using MSE and PSNR metrics
* Compare filter performance analytically

---

## Technologies Used

* Python
* OpenCV
* NumPy
* Matplotlib

---

## Project Structure

```
image_restoration/
│
├── restoration.py
├── images/
├── outputs/
└── README.md
```

---

## Methodology

### 1. Image Preprocessing

* Load surveillance-style images
* Convert images to grayscale

### 2. Noise Modeling

* Gaussian Noise (sensor noise)
* Salt & Pepper Noise (transmission error)

### 3. Image Restoration

Applied spatial filters:

* Mean Filter
* Median Filter
* Gaussian Filter

### 4. Performance Evaluation

Quality measured using:

* Mean Squared Error (MSE)
* Peak Signal-to-Noise Ratio (PSNR)

---

## Observations

* Gaussian filter performs better for Gaussian noise due to smoothing characteristics.
* Median filter effectively removes Salt & Pepper noise while preserving edges.
* Excessive smoothing reduces fine image details.

---

## Outputs

The `outputs/` folder contains:

* Original image
* Noisy images
* Restored images
* Final comparison figure

---

## How to Run

Install dependencies:

```
pip install opencv-python numpy matplotlib
```

Run the program:

```
python restoration.py
```

---

## Conclusion

Image restoration significantly improves surveillance image clarity.
Different noise types require different filters, and performance metrics help in selecting the most suitable restoration technique.

---

## Academic Integrity

This project was implemented individually for academic learning purposes.
References include OpenCV documentation and standard Image Processing textbooks.
