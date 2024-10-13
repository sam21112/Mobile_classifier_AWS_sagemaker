# Mobile Classifier on AWS SageMaker
A machine learning project that involves creating a mobile classifier using AWS SageMaker, showcasing end-to-end deployment and scaling in the cloud.

## Project Overview
This project demonstrates the deployment of a mobile classifier model using AWS SageMaker. It includes scripts for training the model, deploying it as a SageMaker endpoint, and a sample application to interact with the deployed model.

### Features
- **Model Training:** Train a mobile classifier using the provided dataset.
- **Deployment:** Automate the deployment of the machine learning model as a SageMaker endpoint.
- **Prediction:** Utilize the deployed model for making predictions through an API.

## Repository Structure
├── script.py # Training script for the model
├── requirements.txt # Python dependencies required for the project
├── train-V-1.csv # Sample training data
├── test-V-1.csv # Sample test data
├── myenv/ # Virtual environment files and configurations
└── README.md # Documentation of the project


## Getting Started

### Prerequisites
- AWS Account
- Basic knowledge of AWS SageMaker
- Python 3.x

### Setting Up
1. **Clone the Repository**
   ```bash
   git clone https://github.com/sam21112/Mobile_classifier_AWS_sagemaker
   cd Mobile_classifier_AWS_sagemaker
Install Dependencies


pip install -r requirements.txt
Create SageMaker Role

Create an IAM role with SageMaker access and S3 read/write permissions.
Training the Model
Navigate to the AWS SageMaker console.
Create a notebook instance and upload script.py.
Run the training job using the provided dataset.
Deploying the Model
Once the model is trained, deploy it using the SageMaker deployment features.
Use the following command to deploy from your local machine:

python script.py
Usage
Once deployed, you can make predictions by sending requests to the created SageMaker endpoint. Here’s a sample curl request:

curl -X POST https://<endpoint-url> -H 'Content-Type:application/json' -d '{"data": "<input_data>"}'
 
