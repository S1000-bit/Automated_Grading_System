# AWS Bedrock Application

This project leverages AWS Bedrock and Langchain to perform data ingestion, create embeddings, and build a vector store for efficient retrieval-based QA.

## Table of Contents
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Files Description](#files-description)
- [Docker Setup](#docker-setup)
- [License](#license)

## Project Overview

This application demonstrates a complete workflow from data ingestion to embedding creation and QA retrieval using AWS Bedrock and Langchain. The main components include data ingestion, creating vector embeddings, setting up a retrieval-based QA system, and integrating with a Streamlit web interface.

## Installation

### Prerequisites
- Python 3.9+
- AWS Account with access to Bedrock
- Docker (optional, for containerized deployment)

### Steps
1. Clone the repository:
    ```sh
    git clone https://github.com/S1000-bit/Automated_Grading_System.git
    cd Automated_Grading_System
    ```

2. Install the required Python packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

### Running the Application
1. Ensure your AWS credentials are configured. You can configure them using the AWS CLI:
    ```sh
    aws configure
    ```

2. Run the Streamlit application:
    ```sh
    streamlit run main.py
    ```

## Files Description

### `cv.py`
Contains the computer vision-related functionalities, possibly for processing visual data.

### `utils.py`
Utility functions that support the main operations such as data preprocessing, helper functions, etc.

### `main.py`
The main entry point of the application. It sets up the Streamlit interface, handles user inputs, and displays results.

### `Dockerfile`
Defines the Docker image for the application. It includes all the necessary dependencies and setup for containerized deployment.

## Docker Setup

To build and run the application using Docker, follow these steps:

1. Build the Docker image:
    ```sh
    docker build -t aws-bedrock-app .
    ```

2. Run the Docker container:
    ```sh
    docker run -p 8501:8501 aws-bedrock-app
    ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
