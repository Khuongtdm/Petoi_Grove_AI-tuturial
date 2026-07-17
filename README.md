Petoi Grove AI Tutorial
Welcome to the Petoi Grove AI Tutorial! This project provides an accessible, streamlined environment for training and exporting custom object detection models for Petoi robots.

Inspired by the need to make AI vision more approachable, this repository is designed specifically for non-CS users, hobbyists, and educators. It abstracts away the complex setup processes, allowing you to easily pick your model's purpose, train it, and deploy it to your Petoi robot.

✨ Key Features
Beginner-Friendly Training Pipeline: Sets up a ready-to-use environment so anyone can train and export YOLO models without writing complex code.

Multi-Source Dataset Support: Built-in automated scripts to seamlessly download, extract, and format datasets from multiple sources:

Roboflow Universe via API.

Kaggle using kagglehub.

Custom .zip URLs.

Automated Data Formatting: Automatically splits your data into train, val, and test directories, validates YOLO dataset structures, and auto-generates the necessary data.yaml files.

Cloud & Local Compatibility: Run everything easily in the cloud using our provided Google Colab Notebook, or follow the advanced local workspace setup for Windows.

Powered by Ultralytics: Built on top of YOLOv8 (ultralytics==8.4.21) for fast, state-of-the-art object detection.

🚀 Getting Started
Option 1: Cloud Training (Recommended)
The easiest way to get started is by using Google Colab. You don't need a powerful computer—Google provides the GPUs!

Open our Google Colab Notebook.

Follow the step-by-step instructions in the notebook to load your dataset (from Roboflow, Kaggle, or your own files).

Train your model and download the exported weights to use with your Petoi robot.

Option 2: Local Setup (Advanced)
If you prefer to train locally on your own machine with a dedicated GPU:

Clone this repository to your local machine.

Follow the workspace setup script in the tutorial to create an anchored Petoi_Workspace on your drive.

Use the provided Python scripts to structure your datasets and begin local training.

📖 Documentation & Guides
For more detailed explanations, step-by-step labeling guides, and advanced deployment options, please visit our Petoi AI Vision GitBook.

Suggestions for customizing this further:
Add Images: You might want to add an image of a Petoi robot (like Bittle or Nybble) at the top of the README, or a screenshot of the YOLOv8 bounding boxes in action.

Deployment Section: Once you have the code ready for deploying the exported model directly onto the Petoi/Grove hardware, you can add a ## 🤖 Deployment section similar to the EdjeElectronics repository.
