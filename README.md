# Writing the README content to a readme.md file


# Automated Grading Software

This project provides an automated grading system that uses computer vision to assess answer sheets and a BERT transformer model to evaluate written answers based on similarity scores.

## Project Overview

The automated grading software processes scanned answer sheets using OpenCV to identify answer bubbles and written responses. For objective answers (such as multiple-choice), the system detects selected options and grades them based on a predefined answer key. For subjective answers, the project leverages a BERT transformer model to compute a similarity score against model answers, producing a grade based on semantic similarity.

## Features

- **Objective Answer Recognition**: Utilizes OpenCV to locate and identify marked bubbles on scanned answer sheets.
- **Written Answer Grading**: Uses a similarity index based on a BERT transformer to assess written answers against model answers.
- **Automated Grading**: Grades are assigned based on both objective and subjective answer evaluations.

## Project Structure

- **cv.py**: Contains computer vision functions using OpenCV to detect answer bubbles and parse the answer sheets.
- **main.py**: The main script to execute the grading pipeline, combining the CV and NLP components for a comprehensive grading solution.

## Getting Started

### Prerequisites

- Python 3.8+
- OpenCV
- Transformers library (for BERT-based similarity scoring)
- NumPy, Pandas

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/automated-grading-software.git
   cd automated-grading-software
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt

### Contribution

Feel free to submit issues or pull requests to improve the project.

### License

This project is licensed under the MIT License.
 
