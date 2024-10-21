# ScanPlus

> ScanPlus is a healthcare application designed to translate handwritten prescriptions into a digital format. It addresses the issue of illegible handwriting commonly found in medical prescriptions, which can lead to serious errors in patient care. The application uses a deep learning model to classify and extract critical information from prescriptions, including medicine names, dosages, frequency, and diagnostic tests.

## Features
- Translates handwritten medical prescriptions into a digital format.
- Extracts key information such as:
  - **Medicine Names**
  - **Dosages**
  - **Frequency of Use**
  - **Diagnostic Tests**
- Streamlines the process of converting handwritten prescriptions into an easily readable and actionable format for healthcare professionals.
  
## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/ScanPlus.git
    ```

2. **Navigate to the project directory:**
    ```bash
    cd ScanPlus
    ```

3. **Install dependencies:**
    This project requires various libraries, such as TensorFlow (or PyTorch), OpenCV, and others listed in `requirements.txt`. To install all dependencies, run the following:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Train the Model** (optional if pre-trained model is provided):
    - Train the deep learning model using your dataset of handwritten prescriptions. Ensure that the data is labeled correctly for the following categories:
      - Medicine Names
      - Dosages
      - Frequency
      - Diagnostic Tests

    Training and model usage can be configured in `train.py` and `predict.py` respectively.

2. **Run the Application**:
    Once the model is trained and ready, you can run the application to start translating handwritten prescriptions.

    ```bash
    python app.py
    ```

    The app will read the handwritten prescription image, process it, and output the extracted text information.

3. **Input Prescription Image**:
    Provide the prescription image either via the application's interface or by specifying the file path in the code. The deep learning model will analyze the image and convert the handwritten information into a structured digital format.

4. **View Results**:
    The output will display the medicine names, dosages, frequency, and any diagnostic tests mentioned in the prescription.

### Example Input
Upload an image of a prescription with handwritten details, and the application will provide:

- **Medicine Name**: Paracetamol
- **Dosage**: 500 mg
- **Frequency**: Twice a day
- **Diagnostic Test**: Blood Test

## Model Details
The application uses a deep learning model for Optical Character Recognition (OCR) and text classification:
- **OCR** is used to recognize handwritten text.
- The model then classifies the recognized text into predefined categories (medicine names, dosages, etc.).

The model is trained using a labeled dataset of handwritten prescriptions and utilizes advanced neural network architectures to improve accuracy.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.
