# Watcher
Watcher is a work in progress intended to click a button that may show up on the desktop screen. 
The button would be found via the text in the button that appears.
This would be used to accept matches that apear in video games, and then moved on to other practical uses.

Here are the tutorials Watcher is created from:
https://www.pyimagesearch.com/2018/09/17/opencv-ocr-and-text-recognition-with-tesseract/
https://www.pyimagesearch.com/2018/08/20/opencv-text-detection-east-text-detector/

In the future I plan to try and change away from EAST and use the Clova ai detection model.
https://github.com/clovaai/deep-text-recognition-benchmark

Currently I have cobbled together the code from the above tutorials with OpenCV, multithreading, a desktop image grabbing section using Pillow, Tesseract, and mouse automation using PyAutoGUI!
It scans each picture from pillow, runs it through the EAST model to find the text, uses Tesseract to read the text, followed by PyAutoGUI taking control of the system for a second and clicking the button.

