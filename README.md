Dependencies
This project is designed to be run in a Google Colab environment with GPU support. All required Python libraries are installed automatically by the notebook.
torch & torchvision
ultralytics
boxmot
opencv-python
numpy
tqdm
Setup and Installation
The setup process is designed to be as simple as possible.
1. Save the Project Folder to Your Google Drive
You have been provided with a Google Drive folder containing all necessary files (detect).
Action: Please save this entire folder to the root directory of your own Google Drive.
The folder already contains the required structure, including the notebook, the input video, the custom YOLO model, and few output files while training and tuning. It contains the FINAL_1 and FINAL_2 files, which are the last files I worked on for my final model.
2. Open and Run the Colab Notebook
Navigate to the detect folder in your Google Drive and open the Colab notebook file.
Enable the GPU: If not already enabled, go to the menu Runtime → Change runtime type and select T4 GPU from the hardware accelerator dropdown.
The file paths within the notebook are pre-configured to work correctly with this folder structure. No changes are needed.
How to Run the Code
After completing the setup, simply run all the cells of the Colab notebook from top to bottom.
The script will perform the following actions automatically:
Mount your Google Drive.
Install all necessary dependencies.
Load the YOLO and Re-ID models.
Initialise the StrongSORT tracker with the tuned parameters.
Process the input video frame-by-frame, showing a progress bar.
Save the final tracked video to the outputs folder within your project directory.
Upon completion, you will directly see the output file in the drive folder.
