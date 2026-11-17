
# 🎥 Smart Video Background Blur Using YOLO Segmentation & OpenCV

Keep detected objects sharp while automatically blurring the background using AI-powered instance segmentation!

## 📺 YouTube Tutorial

Watch the complete project tutorial on YouTube:

[▶️ Watch the Video](https://youtu.be/kPD7qvFWArQ)

## 🚀 Project Overview

In this project, we build a Smart Video Background Blur system using YOLO Instance Segmentation and OpenCV.

The system detects and segments objects in each video frame using YOLO. It generates a binary mask to separate detected objects from the background.

OpenCV applies Gaussian Blur to the entire frame, while NumPy alpha blending combines the original frame with the blurred frame. The result keeps detected objects sharp and smoothly blurs everything around them.

## ✨ Features

- AI-powered object detection and segmentation using YOLO.
- Automatic binary mask generation.
- Support for multiple detected objects.
- Combine multiple segmentation masks using NumPy.
- Gaussian background blur using OpenCV.
- Sharp object preservation using alpha blending.
- Frame-by-frame video processing.
- Save the final processed video in MP4 format.
- Preview the segmentation mask and final output before processing the complete video.

## 🛠️ Technologies Used

- Python
- YOLO26 Instance Segmentation
- OpenCV
- NumPy
- Matplotlib
- Ultralytics
- TQDM

## ⚙️ How It Works

The complete pipeline follows these steps:

1. Load the YOLO instance segmentation model.
2. Read the input video and extract the first frame.
3. Detect and segment objects in the frame.
4. Generate binary masks for the detected objects.
5. Combine all predicted masks into a single binary mask.
6. Resize the mask to match the original frame dimensions.
7. Apply Gaussian Blur to the original frame.
8. Use NumPy alpha blending to combine the sharp objects and blurred background.
9. Process the remaining video frames.
10. Save the final output video.

## 🎭 Understanding the Segmentation Mask

The binary mask determines which parts of the frame remain sharp and which parts get blurred.

- ⚪ White pixels (255) → Detected objects (Keep Sharp)
- ⚫ Black pixels (0) → Background (Apply Blur)

## 🙌 Support

If you find this project helpful, don't forget to:

- ⭐ Star this repository.
- 👍 Like the YouTube tutorial.
- 🔔 Subscribe for more Computer Vision and AI projects.
- 🍴 Fork this repository and experiment with the code.

## 👨‍💻 Author

Explore more Python, Computer Vision, Deep Learning, and AI projects through my YouTube channel.

📺 [Subscribe on YouTube](https://youtu.be/kPD7qvFWArQ)

---

⭐ If you enjoyed this project, consider giving this repository a star!
