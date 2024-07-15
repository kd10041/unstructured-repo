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

## Additional Resources

- [Unstructured GitHub Repository](https://github.com/Unstructured-IO/unstructured)
- [Official Unstructured Documentation](https://docs.unstructured.io/welcome)

For detailed information and instructions on using the library, consult the official documentation.
