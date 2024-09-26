
# Therapist and Child Detection and Tracking

## Project Description

This project develops a detection and tracking system to identify children and therapists in videos. Using YOLOv5 for object detection and multi-object tracking, it assigns unique IDs to each person. The tool aids in analyzing behaviors, emotions, and engagement levels of children with Autism Spectrum Disorder.

### Features
- Detection of children and therapists in real-time video.
- Unique ID assignment for each detected person.
- Capability to track persons who exit and re-enter the frame.
- Post-occlusion tracking to maintain ID assignment during partial visibility.

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. **Install the required dependencies:**
   Ensure you have Python installed. Then, you can use `pip` to install the required packages.
   ```bash
   pip install -r requirements.txt
   ```

3. **Mount Google Drive (for Colab users):**
   If you are using Google Colab, make sure to mount your Google Drive to access the video files.
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

## Usage

1. Place your input video file in the specified directory:
   - `/content/drive/MyDrive/Assignment-AIMonk_Labs/`
   - Name your video file appropriately.

2. Run the provided Python script:
   ```bash
   python detect_and_track.py
   ```

3. The output video will be saved in the same directory:
   - `output_video.avi`

## Expected Output

The output video will contain:
- Bounding boxes around detected children and therapists.
- Unique IDs displayed above each bounding box.

## Requirements

You will need the following Python packages to run this project:
- `opencv-python`
- `torch`
- `motpy`
- `numpy`
- `PIL`



## Additional Notes

- The YOLOv5 model will be automatically downloaded when you run the code for the first time.
- Make sure your video file format is supported by OpenCV (e.g., `.mp4`, `.avi`).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- YOLOv5 for object detection: [Ultralytics YOLOv5 GitHub](https://github.com/ultralytics/yolov5)
- Motpy for multi-object tracking: [Motpy GitHub](https://github.com/Abdu001/motpy)


![Screenshot 2024-09-26 220459](https://github.com/user-attachments/assets/2ba7bb79-a7b6-4afa-aa8c-e630ee8964f1)


![Screenshot 2024-09-26 220404](https://github.com/user-attachments/assets/c379fdb3-de53-4081-b4a1-5ba6565f00fa)
