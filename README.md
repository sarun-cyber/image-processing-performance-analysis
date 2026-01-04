# Image Processing Performance Analysis

This project analyzes and compares common image processing algorithms from a system performance perspective, focusing on execution time and practical trade-offs.

---

## Overview

Image processing algorithms are widely used in real-world systems such as surveillance, robotics, and embedded vision.  
However, different algorithms provide different trade-offs between output quality and computational cost.

This project benchmarks several commonly used image processing techniques using Python and OpenCV to better understand their performance characteristics.

---

## Problem Statement

When building real-time or resource-constrained systems, selecting the right image processing algorithm is critical.

Some algorithms produce higher-quality results but require more computation time, while others are faster but less accurate.

**This project aims to answer the question:**  
Which image processing algorithms are more suitable for performance-critical systems?

---

## Approach

The project benchmarks multiple image processing algorithms by applying them to the same input image and measuring execution time.

The focus is on **algorithm-level performance**, rather than machine learning or model training.

Workflow:
1. Load a sample image
2. Convert the image to grayscale
3. Apply different image processing algorithms
4. Measure execution time for each algorithm
5. Compare results to identify performance trade-offs

---

## Algorithms Benchmarked

- Sobel Edge Detection
- Canny Edge Detection
- Gaussian Blur
- Median Blur

---

## Project Structure

image-processing-performance/
├── benchmark.py # Benchmark runner
├── algorithms.py # Image processing algorithms
├── sample.jpg # Input image
├── results/
│ └── benchmark.txt # Benchmark results
└── README.md

---

## How to Run

### 1. Install dependencies
```bash
pip install -r requirements.txt

Run benchmark
python benchmark.py

Example Output
Sobel Edge: 0.001480 seconds
Canny Edge: 0.001702 seconds
Gaussian Blur: 0.000165 seconds
Median Blur: 0.002600 seconds

Benchmark results are saved to:
results/benchmark.txt

Why This Project
This project demonstrates:

- Practical performance measurement
- Clean separation between algorithms and benchmarking logic
- System-oriented thinking rather than model-centric approaches
- Realistic evaluation of image processing trade-offs

Possible Extensions

- Benchmark performance at different image resolutions
- Run multiple iterations and analyze variance
- Visualize results using plots
- Add a lightweight web interface for interactive testing
