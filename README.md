# YOLO-World Object Detection
![Yolo-World Logo](https://user-images.githubusercontent.com/your_logo.png)

YOLO-World is a cutting-edge zero-shot object detection model that operates in real-time, leveraging an open-vocabulary framework. 
It is optimized for speed and flexibility, making it approximately 20x faster than traditional zero-shot detectors like GroundingDINO.

## Overview

This project demonstrates how to utilize YOLO-World to detect objects in video files. 
The model supports the dynamic specification of classes through custom prompts, allowing users to adapt it to various domains without retraining. 

### Key Features
- **Zero-Shot Object Detection:** Detect objects without needing labeled training data for each class.
- **Open-Vocabulary Support:** Detect objects using a broad range of categories.
- **Real-Time Inference:** Efficient and quick predictions with low latency.
- **Speed:** Approximately 20x faster than other zero-shot detectors.
- **Customizable Prompts:** Set specific classes to detect without retraining the model.

## Project Structure

- **Installs and Imports:** Necessary libraries and dependencies are installed, including `ultralytics`, `dill`, and `cv2` for video processing and object detection.
- **Configuration (CFG):** The model and video parameters are defined, including the classes to detect, confidence threshold, and input video paths.
- **Video Properties:** A function to extract and display properties of the input video such as frame rate, resolution, and duration.
- **Model Setup:** The YOLO-World model is loaded and customized to detect specific objects defined in the configuration.
- **Inference:** The model runs on the input video, detecting specified objects and saving the output with bounding boxes, labels, and confidence scores.
- **Export Model:** Custom classes are saved into a specialized version of YOLO-World for reuse.
- **Predictions and Detections:** Results are processed and saved, including generating detailed dataframes with detection information and plotting histograms of confidence scores.
- **Visualization:** Detection results are visualized, including the number of detections per class and the confidence histogram.

## Requirements

- Python 
- Libraries: 
  - `ultralytics`
  - `dill`
  - `cv2`
  - `pandas`
  - `seaborn`
  - `matplotlib`

## How to Use

1. **Install Dependencies:**
   - Install the required libraries using pip.
2. **Configure the Model:**
   - Set the desired detection classes, confidence threshold, and video input paths in the configuration section.
3. **Run Inference:**
   - Load the YOLO-World model, set the classes, and run the model on your video input.
4. **Export Results:**
   - Save the results, including the modified model and detection outputs.
5. **Visualize Data:**
   - Generate visualizations to analyze the detection performance and confidence distributions.

## References

- [YOLO-World - Tencent AI Lab](#)
- [YOLO-World Paper - February 2024](#)
- [YOLO-World GitHub](#)
- [YOLO-World - Roboflow Blog](#)
- [YOLO-World - Ultralytics Docs](#)
- [YOLO-World - Hugging Face Space](#)
