# Rock-Paper-Scissors with AI

In this project, you will play the classic game of Rock-Paper-Scissors against an AI opponent. I've created an AI model that is trained to recognize hand gestures using Keras, TensorFlow, and OpenCV. I used OpenCV to gather images and utilized a pretrained model called "SqueezeNet" using the Keras library with TensorFlow as the backend framework.

## Requirements

To run this project, you will need the following software and libraries:

- Python 3
- Keras
- TensorFlow
- OpenCV

## Setup Instructions

Follow these steps to set up and run the project:

1. Clone the repository:

    ```
    git clone https://github.com/your-username/rock-paper-scissors.git
    cd rock-paper-scissors
    ```

2. Download Python 3.7.0 from [here](https://www.python.org/downloads/release/python-370/). Note that you should not add Python 3.7.0 to your PATH during installation.

3. Create a virtual environment for the specific Python version:

    ```
    virtualenv -p <paste_python_3.7_path_location> venv
    ```

4. Activate the virtual environment:

- In Command Prompt (CMD):

  ```
  venv\Scripts\activate.bat
  ```

- In PowerShell:

  ```
  venv\Scripts\Activate.ps1
  ```

5. Install the project dependencies:

    ```
    pip install -r requirements.txt
    ```

6. Gather Images for each gesture (rock, paper, scissors, and none). In this example, we gather 200 images for each gesture. Note that this step is optional:
    ```
    python gather_images.py rock 200
    python gather_images.py paper 200
    python gather_images.py scissors 200
    python gather_images.py none 200
    ```

7. Train the model (optional):
    ```
    python train.py
    ```

8. Test the model on some images:
    ```
    python test.py <file path>.jpg
    ```


9. Play the game against AI:
    ```
    python play.py
    ```

