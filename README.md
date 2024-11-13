
#   	Pedestrian Detection for Autonomous Driving

This project presents a real-time pedestrian detection system for autonomous driving vehicles, employing a YOLO-based deep learning model to recognize and track pedestrians within predefined regions of interest (ROIs) in video frames.
## Description

This design utilizes a deep learning model like YOLO (as implemented in the provided code) for pedestrian detection. A camera mounted on the vehicle captures real-time video feeds, which are processed by YOLO to identify pedestrians in each frame. The YOLO model’s capability to run at high speeds while maintaining accuracy makes it ideal for real-time applications.
## Getting Started

#### Requirements

- Python (>=3.6)
- TensorFlow (>=2.0)
- NumPy
- Matplotlib
- Pandas
- PyTorch
- Opencv2
- Ultralytics
- Supervision
- Tkinter
- TQDM

To use the model, clone this repository to your local machine:

    git clone https: //github.com/VALiiiANT/Pedestrian-Detection-for-Autonomous-Driving

#### Workflow

The project has the following workflow:

1. **Data Preparation:** The dataset is properly formatted and preprocessed. Defined the dataset paths (Train, Test, Val) and specified annotation (Annotations) and image (JPEGImages) directories. Parsed XML files to retrieve label information for each image and used OpenCV to load and resize images to a standardized shape.

2. **Pedestrian Detection and Tracking:** YOLOv8 is loaded with a pre-trained weights file (yolov8x.pt) for detecting people. The model prompts the user to select four points on the first frame of the video to define each ROI. These selections form rectangular zones where pedestrian detection will occur. The video is processed frame-by-frame.

3. **Model Training:** Trained the model over a specified number of epochs, using the validation dataset for performance tracking. 

4. **Model Evaluation:** Captured training and validation metrics (accuracy and loss) to monitor model learning progress and detect potential issues like overfitting.

5. **Performance Analysis:** Defined a function to plot training and validation accuracy and loss over epochs, giving insight into model performance and training progression.

## Results

* An annotated video with the bounding boxes, pedestrian counts, and ROIs is saved in the target directory. Pedestrian counts for each ROI are printed in the console once processing completes.
## Authors
[@AyushiRai](https://github.com/VALiiiANT)

