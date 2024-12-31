Steps:
To clone from github:
mkdir ~/Desktop/Project
cd ~/Desktop/Project


Installations if not there:
pip3 install imutils
pip3 install opencv-python


pip3 uninstall opencv-python-headless
pip3 install opencv-contrib-python


curl -O https://pjreddie.com/media/files/yolov3.weights


python3 -m venv env

source env/bin/activate

pip3 install opencv-python

To run:

Image:
python3 Img_Vid_Webcam.py --image image.png --config yolov3.cfg --weights yolov3.weights --classes yolov3.txt


Video:
python3 Img_Vid_Webcam.py --video video.mp4 --config yolov3.cfg --weights yolov3.weights --classes yolov3.txt

Webcam:

python3 Img_Vid_Webcam.py --webcam  --config yolov3.cfg --weights yolov3.weights --classes yolov3.txt