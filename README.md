
# Video Processing Script

This Python script analyzes a video file to detect and track colored objects, recording their movements across predefined quadrants.

## Setup Instructions

### Requirements

- Python 3.x
- Required Python libraries (`opencv-python`, `opencv-python-headless`, `numpy`)

### Installation

Install the necessary libraries using pip:
```bash
pip install opencv-python opencv-python-headless numpy
```

## Usage

1. Place your video file (`AI Assignment video.mp4`) in the same directory as this script.
2. Adjust the script if your video resolution is different from 1920x1080.
3. Run the script by executing the following command:
   ```bash
   python script_name.py
   ```
4. Follow on-screen instructions to quit the video processing (press 'q' key).

## Functionality

- **Video Processing:** Analyzes each frame of the video to detect specified colors (red, green, blue).
- **Quadrant Detection:** Divides the video frame into quadrants and tracks when objects cross quadrant boundaries.
- **Event Logging:** Records entry and exit events of each colored object into `event_records.txt`.
- **Output:** Generates an output video `output.avi` with bounding boxes and event timestamps overlayed.

## Notes

- Ensure the video file path (`video_path`) is correctly set in the `process_video` function.
- Adjust color ranges and quadrant coordinates as needed for different scenarios.
