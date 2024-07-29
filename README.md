# Bone Fracture Detection

This project is a comprehensive bone fracture detection system utilizing deep learning models. It features a web application built with Flask for image upload and prediction, a desktop GUI built with CustomTkinter for enhanced user interaction, and robust training scripts for model development and testing.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
  - [Web Application](#web-application)
  - [Desktop GUI](#desktop-gui)
- [Model Training](#model-training)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)

## Installation

### Prerequisites

Ensure you have the following installed:
- Python 3.8 or later
- Pip
- Virtual environment (optional but recommended)

### Steps

1. **Clone the Repository**
   ```sh
   git clone https://github.com/yourusername/bone-fracture-detection.git
   cd bone-fracture-detection
   ```

2. **Create and Activate a Virtual Environment**
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the Required Packages**
   ```sh
   pip install -r requirements.txt
   ```

4. **Download Pretrained Models**
   Place the pretrained models in the `weights` folder. Ensure the following models are available:
   - ResNet50_Elbow_frac.h5
   - ResNet50_Hand_frac.h5
   - ResNet50_Shoulder_frac.h5
   - ResNet50_BodyParts.h5

## Usage

### Web Application

1. **Run the Flask App**
   ```sh
   python app.py
   ```

2. **Access the Web Application**
   Open a browser and navigate to `http://127.0.0.1:5000/`.

3. **Upload and Predict**
   - Upload an X-ray image.
   - View the prediction results indicating the bone type and fracture status.

### Desktop GUI

1. **Run the GUI Application**
   ```sh
   python maingui.py
   ```

2. **Interact with the GUI**
   - Upload an X-ray image.
   - Click on the "Predict" button to get the bone type and fracture status.
   - View and save the prediction results.


## Contributing

Contributions are welcome! Please fork this repository and submit pull requests for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
