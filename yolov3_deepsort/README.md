# Player Tracking with Statistics Display (using Yolo-v3 and DeepSort)
For this part of the project, our code is based on the [existing open-source tool written by The AI Guy](https://github.com/theAIGuysCode/yolov3_deepsort).

## Set Up
Download official pretrained weights either using `wget https://pjreddie.com/media/files/yolov3.weights -O weights/yolov3.weights` or directly from [here](https://pjreddie.com/media/files/yolov3.weights). Then put `yolov3.weights` under `yolov3_deepsort/weights`.

## Our Contribution
1. Integrated the environment with the rest of the backend
2. Calculate the instant speed of each player
3. Display the statistics along the tracking result
4. Split this functionality out as an option to enhance user experience

## Image Demo
<img src="https://github.com/AJ-Wuu/SoccerNetPlus/blob/main/video_output/tracking-screenshot.png" alt="tracking-demo" />
