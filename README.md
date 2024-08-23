# Face Recognition Attendance System

## Overview
This Python program uses OpenCV and face_recognition libraries to capture video from your webcam, detect faces, and mark attendance by saving the recognized faces' names and the time they were detected into a CSV file.

## Requirements
- Python 3.x
- OpenCV
- face_recognition
- numpy

## Installation Steps

1. **Install Python 3.x**
   - Download and install Python from [python.org](https://www.python.org/).
   - Make sure to add Python to your PATH during the installation process.

2. **Set Up a Virtual Environment (Optional but Recommended)**
   - Navigate to your project directory and run:
     ```sh
     python -m venv venv
     ```
   - Activate the virtual environment:
     - **Windows:** `venv\Scripts\activate`
     - **macOS/Linux:** `source venv/bin/activate`

3. **Install Required Python Libraries**
   - Run the following command to install the necessary packages:
     ```sh
     pip install opencv-python face_recognition numpy
     ```

4. **Place the Required Images**
   - Create a directory named `photos` in the same folder as your script.
   - Add the images of the people you want to recognize, ensuring that the filenames correspond to the person’s name. For example, `photos/jobs.jpg` for "Steve Jobs" and `photos/shiva.jpg` for "Shiva."

5. **Run the Program**
   - Execute the script:
     ```sh
     python your_script_name.py
     ```

6. **Mark Attendance**
   - The program will automatically detect faces and mark attendance by logging the person's name and the time into a CSV file named with the current date (e.g., `2024-08-23.csv`).

## Common Issues & Troubleshooting

1. **ModuleNotFoundError: No module named 'cv2'**
   - Ensure that OpenCV is installed. Run `pip install opencv-python` and check if the issue persists.
   
2. **ModuleNotFoundError: No module named 'face_recognition'**
   - Make sure you have installed the face_recognition library correctly. Run `pip install face_recognition`.

3. **Webcam Not Working**
   - Check if your webcam is properly connected.
   - Ensure that no other application is using the webcam.
   - If you're using a virtual environment, make sure you have the correct version of Python and OpenCV installed.

4. **Faces Not Being Recognized**
   - Ensure that the images in the `photos` directory are clear and only contain one face.
   - If the face is not being detected, try adjusting the image size or brightness.

5. **Script Exits Immediately**
   - Make sure you are not accidentally pressing the 'q' key, which is set to quit the program.
   - Verify that your webcam is working and that the program is receiving video input.

## Screenshots
**Main Program Running:**
![Main Program](screenshot1.png)

**Face Detection:**
![Face Detection](screenshot2.png)

**Attendance Marked in CSV:**
![CSV Output](screenshot3.png)

