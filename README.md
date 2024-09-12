# PAN Card Tampering Detection

This project demonstrates a technique for detecting tampering in PAN card images using image processing techniques. The approach involves comparing an original image of a PAN card with a potentially tampered image using Structural Similarity Index (SSIM) and visualizing differences through various image processing techniques.

## 📸 Project Overview

- **Objective:** Detect tampering in PAN card images by comparing an original and a tampered image.
- **Techniques Used:** Image resizing, format conversion, Structural Similarity Index (SSIM), contour detection, and image visualization.

## 🔧 Prerequisites

- Python 3.8 or higher
- Required libraries: `numpy`, `opencv-python`, `scikit-image`, `Pillow`, `requests`, `imutils`

## 🛠️ Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/pan-card-tampering-detection.git
    cd pan-card-tampering-detection
    ```

2. **Create and activate a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages:**

    ```bash
    pip install numpy opencv-python scikit-image Pillow requests imutils
    ```

## 🚀 Usage

1. **Run the script:**

    The script performs the following operations:
    - Fetches the original and tampered PAN card images.
    - Resizes and converts images as necessary.
    - Computes SSIM to evaluate the similarity between the images.
    - Detects differences using contours and generates various visualizations.

    ```bash
    python your_script_name.py
    ```

2. **View Results:**

    The script will save the following images in the `pan_card_tampering/image` directory:
    - `original.png`: The original PAN card image.
    - `tampered.png`: The tampered PAN card image.
    - `original_contour_image.png`: Original image with contours highlighting differences.
    - `tampered_contours_image.png`: Tampered image with contours highlighting differences.
    - `difference_image.png`: Difference image showing changes between original and tampered images.
    - `threshold_image.png`: Threshold image showing the detected regions of difference.

## 📄 Code Explanation

- **Image Loading:** The images are fetched from URLs and loaded using `Pillow`.
- **Resizing & Conversion:** Both images are resized to a common dimension and converted to the same format.
- **SSIM Calculation:** The Structural Similarity Index (SSIM) is computed to quantify the similarity between the two images.
- **Contour Detection:** Contours are detected in the difference image to highlight tampered areas.
- **Visualization:** Various images are saved to visualize the differences and contours.

## 🛡️ Security Note

Ensure you handle image data responsibly and avoid using sensitive or personal information in test cases.

## 🤝 Contributions

Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

For questions or suggestions, feel free to reach out to [Your Name](https://www.linkedin.com/in/karthikbs85/) on LinkedIn.
