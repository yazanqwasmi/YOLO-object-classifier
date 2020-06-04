# YOLO-object-classifier
Commands:

For real time object classification:

Step one: enter directory of your file using terminal, cmd or equivalent. 

cd ~/*directory command* eg (cd ~/Desktop/real-time-object-detection)

Step two: define inputs into model.

command = % python real_time_object_detection.py \
        --prototxt MobileNetSSD_deploy.prototxt.txt \
        --model MobileNetSSD_deploy.caffemodel
        
        
        
For image input classification: 

Step one: enter directory of your file using terminal, cmd or equivalent. 
cd ~/*directory command*       eg (cd ~/Desktop/yolo-object-detection)

Step two: define inputs into model.
%python yolo.py --image images/baggage_claim.jpg --yolo yolo-coco


For video input classification:
Step one: enter directory of your file using terminal, cmd or equivalent. 

cd ~/*directory command*       eg (cd ~/Desktop/yolo-object-detection)

Step two: define inputs into model.
python yolo_video.py --input videos/car_chase_01.mp4 \
--output output/car_chase_01.avi --yolo yolo-coco
