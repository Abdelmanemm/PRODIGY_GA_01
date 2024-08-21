# PRODIGY_GA_01

## Overview
This project is a fine-tuned GPT-2 model designed to generate jokes based on user-provided prompts. The model has been trained on a dataset of jokes to generate humorous responses and has been deployed using a FastAPI framework. This README file provides a comprehensive guide to the project, including how to set up, use, and contribute to the repository.

## Table of Contents
1. [Project Structure](#project-structure)
2. [Installation](#installation)
3. [Usage](#usage)
4. [API Documentation](#api-documentation)
5. [Model Details](#model-details)
6. [Examples](#examples)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact](#contact)

## Project Structure
```
gpt2-joke-generator/
│
├── src/
│ ├── init.py # Initializes the src module
│ ├── main.py # Main entry point of the API
│ ├── utils.py # Utility functions for data processing and model handling
│ └── api.py # FastAPI setup and route definitions
│
├── model/
│ └── checkpoint-30000/ # Directory containing the fine-tuned GPT-2 model
│
├── data/
│ └── jokes.csv # Dataset used for fine-tuning the model
│
├── requirements.txt # Python dependencies required to run the project
├── README.md # Project documentation
└── .gitignore # Git ignore file
```
## Installation

To set up the project locally, follow these steps:

1. **Clone the repository:**
   ```
   git clone https://github.com/yourusername/gpt2-joke-generator.git
   cd gpt2-joke-generator
   ```
2. **Create Virtual enviroment**
   ```
   python3 -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   ```
3. **Install requirements**
   ```
   pip install -r requirements.txt
   ```
4. Download pretrained model
   sorry but the fine tuned model size is about 3.96 GB which I can't upload on
   github due to size limitaions just download data and apply process_data.py file
   and then use the output and run training.ipynb notebook it will save the model
   checkpoint  in ./results directory you can later use this to run the api 
   
