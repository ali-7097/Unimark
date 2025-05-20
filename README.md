# UniMark - Facial Recognition Attendance Management System

UniMark is an intelligent attendance management system that uses facial recognition technology to automatically mark student attendance in educational institutions.

## Features

- **Student Management**: Add, update, and manage student information
- **Facial Recognition**: Automatically mark attendance using face detection
- **Attendance Records**: View and manage attendance data
- **AI Model Training**: Train the facial recognition model with student images

## Project Structure

- `code/`: Contains all Python source files
  - `UniMark.py`: Main application entry point
  - `Unimark_Student.py`: Student management module
  - `Unimark_Face_Recog.py`: Facial recognition module
  - `Unimark_Attendance.py`: Attendance management module
  - `Unimark_train_ai.py`: AI model training module
- `Data/`: Stores student data and images
- `Images for GUI/`: Contains GUI images and icons
- `classifier.xml`: Trained model for facial recognition
- `haarcascade_frontalface_default.xml`: Haar cascade classifier for face detection

## Requirements

- Python 3.7+
- tkinter (for GUI)
- PIL (Python Imaging Library/Pillow)
- OpenCV (cv2)
- numpy
- pandas

## Installation

1. Clone or download this repository
2. Create a virtual environment (recommended)
   ```
   python -m venv env
   ```
3. Activate the virtual environment
   - Windows: `env\Scripts\activate`
   - Linux/Mac: `source env/bin/activate`
4. Install required packages
   ```
   pip install opencv-python
   pip install pillow
   pip install numpy
   pip install pandas
   ```

## Usage

1. Activate your virtual environment
2. **Important**: Update image paths in code files
   - The code currently uses absolute paths for images (e.g., `r"C:\NUST\1ST Semester\ICT\End Semester Project\Images for GUI\background image.jpg"`)
   - Update these paths in `UniMark.py` and other files to match your system's directory structure
3. Run the main application
   ```
   python code/UniMark.py
   ```
4. Use the GUI to navigate between different modules:
   - "Student Details" to manage student information
   - "Train Model" to train the facial recognition model
   - "Facial Recognition" to detect faces and mark attendance
   - "Attendance" to view and manage attendance records

## Important Notes

- This application requires a webcam for facial recognition functionality
- The facial recognition accuracy depends on proper lighting conditions
- Make sure all image paths in the code are correctly set up for your system
- The classifier.xml file is required for the facial recognition to work properly

## Workflow

1. First, add student information using the "Student Details" module
2. Capture student face samples during registration
3. Train the facial recognition model using the "Train Model" module
4. Use the "Facial Recognition" module to detect students and mark attendance
5. View and export attendance records from the "Attendance" module

## Troubleshooting

If the application fails to start:
1. Check that all dependencies are properly installed
2. Verify image paths are correctly updated to match your system
3. Ensure the virtual environment is activated when running the application 
