# STC-2025: SoccerTrack Challenge 2025 
[![Discord](https://img.shields.io/badge/Discord-Join%20Chat-5865F2?logo=discord&logoColor=white)](https://discord.gg/yDrcywCs)

## Overview 
The SoccerTrack Challenge 2025 @MMSports2025 is a competition designed to advance the tracking of soccer players in fixed-viewpoint video footage. Participants will be provided with a dataset containing match footage annotated with bounding boxes and player IDs for training.

During the test phase and the final challenge phase, participants will be given unseen match footage, where they must perform player tracking and submit their results. The ranking will be determined based on the performance of their tracking models on this unseen data.

## Dataset  
The Dataset for this challenge are SoccerTrack-v2 datasets. 

**Data Source:** The complete dataset is available at: [google drive](https://drive.google.com/drive/folders/1_o78gcL4j0xHxbRjSR1Evs4VLXCr2ncD).

---

## Official Website  
[SoccerTrack Challenge 2025 Official Site](https://sites.google.com/g.sp.m.is.nagoya-u.ac.jp/stc2025)
---

## How to Use 
[stc_baseline_no_finetune.ipynb](https://colab.research.google.com/github/Yinlipp/SoccerTrackChallenge-2025_Colab/blob/main/stc_baseline_no_finetune.ipynb) is a baseline Google Colab code for the SoccerTrack Challenge 2025, without fine-tuning.

The code is divided into two parts: 
(Participants can ignore the second part, only the MOT-format .txt tracking results from the first part need to be submitted.)

1.Using the official Deep-EIoU code (https://github.com/hsiangwei0903/Deep-EIoU) to perform tracking on videos and obtain tracking results in MOT-format .txt files.
The video should be in .mp4 format. You can replace it with your own by providing a video link or uploading the file to the appropriate folder.
After running Cell 1, you will obtain both the tracking result in MOT-format .txt and the corresponding output video in .mp4 format.

2.Using the official HOTA code (https://github.com/JonathonLuiten/TrackEval)to evaluate the tracking results from part 1 with the ground truth using the HOTA metric.
Place the tracking result .txt files and ground truth files according to the directory structure required by TrackEval in order to compute the HOTA metric.

3.[Fine-tune baseline](https://github.com/Yinlipp/STC-2025-SoccerTrack-Challenge_Finetune)
## Author of the code
- [YIN Li](https://github.com/Yinlipp)

## Reference
- [Deep-EIoU](https://github.com/hsiangwei0903/Deep-EIoU)  
- [TrackEval (HOTA)](https://github.com/JonathonLuiten/TrackEval)

