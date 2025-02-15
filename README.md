# TB Detection System

An AI-powered application that analyzes chest X-rays to detect tuberculosis. This system integrates deep learning with blockchain technology for secure record-keeping.

## Features
- AI-based TB detection from X-ray images
- Web-based user interface
- Blockchain record storage for secure data management
- 9-class TB classification using a CNN model

## System Requirements
### Software Requirements
- Python 3.x
- TensorFlow
- Flask
- OpenCV
- Web3.py
- Ganache (for blockchain simulation)

### Hardware Requirements
- Minimum 8GB RAM
- Storage space for model files (~100MB)
- GPU (optional but recommended)

## Installation Guide
1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-repo/tb-detection.git
   cd tb-detection
   ```
2. **Install dependencies:**
   ```sh
   pip install tensorflow flask opencv-python web3 numpy
   ```
3. **Install Ganache for blockchain simulation.**

## Project Structure
```
project/
├── app.py (Main Flask application)
├── model.py (AI model implementation)
├── templates/
│   ├── index.html (Upload interface)
│   └── result.html (Results display)
├── static/
│   └── uploads/ (Image storage)
└── blockchain/
    └── contracts/ (Smart contracts)
```

## Running the Application
### 1. Start the Blockchain
Open a terminal, navigate to the `blockchain` folder, and run:
```sh
npx ganache
```

### 2. Start the Flask Application
Open another terminal, navigate to the `tb_detection_web` folder, and run:
```sh
python app.py
```

### 3. Access the Web Interface
Go to:  
```sh
http://localhost:5000
```
Upload an X-ray image to analyze TB and view the blockchain record.

## Troubleshooting
- **Model Loading Error:** Ensure `full_model.h5` exists in the correct directory.
- **Blockchain Connection Issues:** Check if Ganache is running.
- **Upload Errors:** Verify permissions for the upload directory.

## Security Considerations
- Secure file upload handling
- Blockchain transaction security
- Data privacy measures
- Access control implementation

## License
This project is licensed under the MIT License.

## Contact
For issues and contributions, please create an issue or submit a pull request.
