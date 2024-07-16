# Unstructured-Repo

## Installation Steps

1. **Create a Virtual Environment:**
   * Set up a new virtual environment using pip or miniconda.

2. **Install Unstructured Library with PDF Support:**
   * Run:
     ```
     pip install "unstructured[pdf]"
     ```

3. **Additional Dependencies:**
   * Ensure the following are installed:
     * **poppler-utils:** To handle images and PDFs.
       - For installation instructions, refer to [this StackOverflow post](https://stackoverflow.com/questions/18381713/how-to-install-poppler-on-windows).
     * **tesseract-ocr:** Required for PDF and image processing. 
       - For installation instructions on Windows, refer to [this StackOverflow post](https://stackoverflow.com/questions/46140485/tesseract-installation-in-windows).
       - Install tesseract-lang for extra language support.

## Repository Contents

This repository includes code and sample test PDF files for evaluating the unstructured library.

## Available Models for Partitions

Unstructured provides several models for partitioning documents:

* **detectron2_onnx**: A Computer Vision model by Facebook AI that provides object detection and segmentation algorithms with ONNX Runtime. It is the fastest model with the `hi_res` strategy.
* **yolox**: A single-stage real-time object detector that modifies YOLOv3 with a DarkNet53 backbone.
* **yolox_quantized**: Runs faster than YoloX and its speed is closer to Detectron2.

Based on testing with the sample PDFs in this repository, `yolo_quantized` provided the best results.

For more detailed information about these models and their usage, refer to the [Unstructured Models Documentation](https://docs.unstructured.io/open-source/concepts/models).

## Additional Resources

- [Unstructured GitHub Repository](https://github.com/Unstructured-IO/unstructured)
- [Official Unstructured Documentation](https://docs.unstructured.io/welcome)

For detailed information and instructions on using the library, consult the official documentation.
