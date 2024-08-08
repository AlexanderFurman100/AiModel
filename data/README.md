READ THIS BEFORE USING:
-

This machine learning model uses a ResNet-18 algorithm along with a CNN (Convolutional Neural Network) in order to determine whether an image is of plastic or of paper. This can be used to automate sorting, or to help somebody know what can be recycled or not. The dataset is a collection of various images found on the internet. The data is split into three folders/categories: train, val (validate), and test. The train folder is what the model uses to learn, the val folder helps validate the model's accuracy, and the test folder contains images that can be used to test the model's accuracy. This project is intended for use with python, and specifically on an NVIDIA Jetson Nano. To run, all files in the repository must be downloaded and saved on a linux machine. Once you are in the folder continting the files on the linux machine, run this command: imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/file.jpg output.jpg


DIRECTIONS FOR USE:

At the end of the code, where it says, "file.jpg", replace "file.jpg" with the name of the image you want to have the model to analyze, while keeping the part that says, "output.jpg" To have the model analyze an image not currently included in the test folder, you can upload your own image into the test folder and run the command with the name of your image. Alternatively, you can replace "file.jpg" with, "plastic/file.jpg" or "paper/file.jpg", where "file.jpg" is one of the images provided in the chosen folder (plastic or paper). To view the model's outcome, open the file titled, "output.jpg".

Link to demonstration: https://drive.google.com/file/d/1nGKWddWmkRCodx1CwQlyNHEp_mJCJ3Y8/view?usp=sharing
