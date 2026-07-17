# Petoi Grove AI Tutorial

Welcome to the **Petoi Grove AI Tutorial**! This project provides an accessible, streamlined environment for training and exporting custom object detection models for Petoi robots. 

Inspired by the need to make AI vision more approachable, this repository is designed specifically for non-CS users, hobbyists, and educators. It abstracts away the complex setup processes, allowing you to focus on training powerful vision models for your robots.

## ✨ Key Features

*   **Beginner-Friendly Training Pipeline:** Sets up a ready-to-use environment so anyone can train and export YOLO models without writing complex code.
*   **Multi-Source Dataset Support:** Built-in automated scripts to seamlessly download, extract, and format datasets from multiple sources:
    *   [Roboflow Universe](https://universe.roboflow.com/) via API.
    *   [Kaggle](https://www.kaggle.com/) using `kagglehub`.
    *   Custom `.zip` URLs.
*   **Automated Data Formatting:** Automatically splits your data into `train`, `val`, and `test` directories, validates YOLO dataset structures, and auto-generates the necessary `data.yaml` files.
*   **Cloud & Local Compatibility:** Run everything easily in the cloud using our provided [Google Colab Notebook](https://colab.research.google.com/drive/1aI8qhm68j9JntMN_tRY9NFXVe6mNuoJP), or follow guided local setup.
*   **Powered by Ultralytics:** Built on top of YOLOv8 (`ultralytics==8.4.21`) for fast, state-of-the-art object detection.

## 🚀 Getting Started

### Option 1: Cloud Training (Recommended)
The easiest way to get started is by using Google Colab. You don't need a powerful computer—Google provides the GPUs!
1. Open our [Google Colab Notebook](https://colab.research.google.com/drive/1aI8qhm68j9JntMN_tRY9NFXVe6mNuoJP).
2. Follow the step-by-step instructions in the notebook to load your dataset (from Roboflow, Kaggle, or your own files).
3. Train your model and download the exported weights to use with your Petoi robot.

### Option 2: Local Setup (Advanced)
If you prefer to train locally on your own machine with a dedicated GPU:
1. Open our [Google Colab Notebook](https://colab.research.google.com/drive/1aI8qhm68j9JntMN_tRY9NFXVe6mNuoJP).
2. Follow the workspace setup script in the tutorial "Local setup"
3. Use the provided Python scripts to structure your datasets and begin local training.
4. Switch back to the cloud environment to export (also in the GitBook)

## 🤖 Deploying AI Vision to Your Petoi Robot

Once you've trained your custom object detection model, the next step is deploying it to your Petoi robot for real-world vision capabilities.

### Deployment Overview
*   **Model Export:** Your trained YOLOv8 model is automatically converted to optimized formats suitable for the Petoi platform.
*   **Lightweight Inference:** The exported model runs efficiently on Petoi's embedded hardware, enabling real-time object detection without significant latency.
*   **Integration with Petoi Firmware:** Seamlessly integrate your custom vision model into the robot's control system for autonomous decision-making.
*   **Multi-Model Support:** Deploy multiple specialized models for different detection tasks (e.g., person detection, obstacle avoidance, target tracking).

### Deployment Steps
1. Follow instruction in the link: [Petoi AI Vision](https://docs-example.gitbook.io/petoi-ai-vision/advanced-development-and-application-of-ai-vision-modules/deploy-model-to-sensecraft)

### Hardware Requirements
*   **Petoi Robot Series:** Compatible with all current Petoi models with embedded vision capability.
*   **Storage:** Ensure sufficient onboard storage (typically 50-200MB depending on model complexity).
*   **Compute:** Petoi's built-in accelerator handles real-time inference efficiently.

### Performance Optimization
*   **Model Quantization:** Reduce model size and inference time through post-training quantization techniques.
*   **Batch Processing:** Configure batch inference for multiple detection frames per second.
*   **Confidence Thresholding:** Fine-tune detection confidence to balance accuracy and speed based on your use case.

## 📖 Documentation & Guides

For more detailed explanations, step-by-step labeling guides, deployment walkthroughs, and advanced configuration options, please visit our [Petoi AI Vision GitBook](https://docs-example.gitbook.io/petoi-ai-vision).

For specific deployment troubleshooting, refer to the [Deployment Troubleshooting Guide](https://docs-example.gitbook.io/petoi-ai-vision/deployment/troubleshooting).
