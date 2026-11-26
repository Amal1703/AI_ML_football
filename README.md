# AI_ML_football

- yolo_model.zip: contains best.pt (the YOLO 11 model after training in stage_1.ipynb)

- football-players-detection-20.zip: contains 3 folders — train, test, and validation — with images and labels for player, referee, goalkeeper, and ball. (I downloaded it from roboflow.com; see stage_1.ipynb)

- input_data.zip: Contains a video named 08fd33_4.mp4, downloaded from https://drive.google.com/file/d/1t6agoqggZKx6thamUuPAIdN_1zR9v9S_/view. This is a football game video that we will work on

- output_data_after_yolo_prediction.zip: Contains a video named 08fd33_4.mp4, which is the output of the trained YOLO model applied to the input video 08fd33_4.mp4 (from input_data.zip). See stage_1.ipynb.

- track_stubs.pkl

- stage_1_train_YOLO_model.ipynb

- stage_2.ipynb

-
- As you can see in the video in output_data_after_yolo_prediction (Contains a video named 08fd33_4.mp4, which is the output of the trained YOLO model applied to the input video 08fd33_4.mp4 (from input_data.zip)), the same referee or goalkeeper is detected as a player, or vice versa. In the Image_explaining_why_data_preprocessing_is_needed_after_YOLO_+_Tracker folder, we have example images showing a player being assigned the same ID across multiple frames — but it is not always the same player. This is an ID switch / ID mismatch problem produced by the tracker. Therefore, we need to do Data Preprocessing.
