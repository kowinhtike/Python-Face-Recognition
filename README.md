# Face Recognition Project

This project uses `face_recognition` and `OpenCV` to recognize known faces via a webcam in real-time.

## Requirements

- Python 3.7+
- OpenCV
- dlib
- face_recognition
- NumPy

## Installation

1️⃣ **Install CMake Manually**
   - Download CMake from the [official site](https://cmake.org/download/).
   - Choose **Windows x64 Installer**.
   - Install CMake and check **"Add CMake to system PATH"** during installation.
   - Restart your terminal (cmd or PowerShell).
   - Verify installation:
     ```bash
     cmake --version
     ```
     🎯 If it shows a version number, CMake is installed correctly!

2️⃣ **Install Visual Studio Build Tools**
   - `dlib` needs C++ Build Tools to compile.
   - Download & install **Visual Studio Build Tools**.
   - During installation, select:
     - **C++ CMake Tools for Windows**
     - **MSVC v142 - VS 2019 C++ x64/x86 build tools**
     - **Windows 10 SDK**
   - Restart your PC after installation.

3️⃣ **Upgrade Pip & Install Dependencies**
   - Run these commands in your virtual environment:
     ```bash
     python -m pip install --upgrade pip setuptools wheel
     pip install cmake dlib face-recognition opencv-python numpy
     ```
     🚀 This should install everything without errors!

4️⃣ **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/face-recognition-project.git
   cd face-recognition-project
   ```

5️⃣ **Create a virtual environment (optional but recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

6️⃣ **Install additional dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Add known faces**
   - Place images of known people in the project folder.
   - Update the script with the image file names and corresponding names.

2. **Run the program**
   ```bash
   python face_recognition_live.py
   ```

3. **Press `q` to quit**

## Troubleshooting

- If `face_recognition` installation fails on Windows, ensure `dlib` is properly installed.
- Ensure that `cv2` (OpenCV) is correctly installed.

## Notes

- Adjust the `tolerance` parameter in `face_recognition.compare_faces()` for better accuracy.
- For performance improvement, resize the webcam input frame before processing.


