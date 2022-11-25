# Player Detection with Birdeye 2D Transformation (using Yolo-v3 and OpenCV)

## Set Up
Download official pretrained weights either using `wget https://pjreddie.com/media/files/yolov3.weights -O models/yolov3.weights` or directly from [here](https://pjreddie.com/media/files/yolov3.weights). Then put `yolov3.weights` under `yolov3_opencv/models`.

## Our Contribution
1. Find fixed-angle video as training resources (because OpenCV cannot be directly applied on moving-angle videos) from [ISSIA Dataset](http://ipl.ce.sharif.edu/ball_datasets.html)
2. Use Yolo-v3 to identify people and the ball, and get the coordinates
3. Distinguish people based on their roles (judges🟥🟨 or players⚽) and teams (honestly I don't know the name of the teams, but we all know there are always two teams 🤣) with different color of rectangles
4. Transform the players' spot on a 2D digital field -- this could potentially be very useful for users learning the team's strategy, players' relative positions and some general rules like offside
5. Split this functionality out as an option to enhance user experience

## Image Demo
<img src="https://github.com/AJ-Wuu/SoccerNetPlus/blob/main/video_output/detection-screenshot.png" alt="detection-demo" />
<img src="https://github.com/AJ-Wuu/SoccerNetPlus/blob/main/video_output/birdeye-screenshot.png" alt="birdeye-demo" />
