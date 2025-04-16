# SoccerTrackChallenge-2025_Colab
The stc_baseline_no_finetune.ipynb is a Baseline Colab code for the SoccerTrack Challenge 2025 (STC-2025), without fine-tuning.

The code is divided into two parts: 
(Participants can ignore the second part, only the MOT-format .txt tracking results from the first part need to be submitted.)

1.Using the official Deep-EIoU code (https://github.com/hsiangwei0903/Deep-EIoU) to perform tracking on videos and obtain tracking results in MOT-format .txt files.
The video should be in .mp4 format. You can replace it with your own by providing a video link or uploading the file to the appropriate folder.
After running Cell 1, you will obtain both the tracking result in MOT-format .txt and the corresponding output video in .mp4 format.

2.Using the official HOTA code (https://github.com/JonathonLuiten/TrackEval)to evaluate the tracking results from part 1 with the ground truth using the HOTA metric.
Place the tracking result .txt files and ground truth files according to the directory structure required by TrackEval in order to compute the HOTA metric.

## Reference
- [Deep-EIoU](https://github.com/hsiangwei0903/Deep-EIoU)  
- [TrackEval (HOTA)](https://github.com/JonathonLuiten/TrackEval)

