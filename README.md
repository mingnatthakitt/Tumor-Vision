# TumorVision

[Check out our demo](https://btis-tumorvision.streamlit.app)

TumorVision is an innovative tool designed to empower healthcare professionals in the diagnosis of brain tumors. By leveraging a cutting-edge machine learning model, this application provides rapid and accurate identification of various brain tumor types from MRI scans.

Our mission is to enhance patient outcomes by enabling prompt and precise diagnoses, serving as a crucial initial step in the treatment process. TumorVision is more than just an AI tool; it's a vital aid in the fight against terminal illnesses, helping to alleviate disease impact through early and accurate detection.

## Key Features

-   **Advanced AI Model:** Utilizes a powerful `EfficientNetV2-S` model, fine-tuned on the Brain Tumor Image Set (BTIS), to achieve high diagnostic accuracy.
-   **Rapid Identification:** Delivers predictions for brain tumor types from MRI images in seconds.
-   **Top-3 Probability Scores:** Displays the three most likely tumor types with their corresponding probabilities, providing a comprehensive analysis to aid diagnostic confidence.
-   **Informative Tumor Guide:** Includes a dedicated page with descriptions for all 14 tumor types the model can identify.
-   **User-Friendly Web App:** Built with Streamlit for a clean, intuitive, and easy-to-use interface for uploading images and viewing results.

## Tumor Types Detected

The model is trained to classify 15 different categories, including 14 distinct tumor types and normal brain scans. These include:

-   Astrocitoma
-   Carcinoma
-   Ependimoma
-   Ganglioglioma
-   Germinoma
-   Glioblastoma
-   Granuloma
-   Meduloblastoma
-   Meningioma
-   Neurocitoma
-   Oligodendroglioma
-   Papiloma
-   Schwannoma
-   Tuberculoma
-   Normal

## Technology Stack

-   **Backend:** Python
-   **ML/DL Framework:** TensorFlow, Keras
-   **Web Framework:** Streamlit
-   **Core Libraries:** OpenCV, Pillow, NumPy

## Getting Started

To run this project locally, please follow the steps below.

### Prerequisites

-   Python 3.8+
-   pip
-   Git LFS (for downloading the large model files)

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/mingnatthakitt/TumorVision.git
    cd TumorVision
    ```

2.  **Install Git LFS and pull the model files:**
    ```bash
    git lfs install
    git lfs pull
    ```
    *Note: The model files (`.h5`) are large and require Git LFS to be properly downloaded.*

3.  **Install the required Python packages:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Streamlit application:**
    ```bash
    streamlit run main.py
    ```
    The application will open in your default web browser.

## How to Use

1.  Launch the application and navigate to the **TumorVision** page from the navigation bar.
2.  Drag and drop or browse your files to upload an MRI image of a brain (`.jpg`, `.png`, or `.jpeg`).
3.  Wait a few moments for the model to analyze the image.
4.  The application will display the uploaded image and the top three predictions with their confidence probabilities.

## Running with a Dev Container

This repository is configured for development containers. You can easily run the project in a containerized environment like GitHub Codespaces or using the VS Code Dev Containers extension.

1.  Open the repository in GitHub Codespaces or in VS Code with the Dev Containers extension installed.
2.  The container will automatically build, install all dependencies from `requirements.txt`, and start the Streamlit application.
3.  A port will be forwarded, and you can open the application directly in a browser tab.
