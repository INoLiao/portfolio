---
layout: page
title: Projects
nav_order: 2
---

# Projects

---

<h3><a href="https://inoliao.github.io/CoachAI/" target="_blank">TrackNet: A Deep Learning Network for Tracking High-speed and Tiny Objects in Sport Applications</a></h3>
<div align="justify">
Ball trajectory data are one of the most fundamental and useful information in the evaluation of players' performance and analysis of game strategies. Although vision-based object tracking techniques have been developed to analyze sport competition videos, it is still challenging to recognize and position a high-speed and tiny ball accurately. In this work, we develop a deep learning network, called TrackNet, to track the badminton from broadcast videos in which the ball images are small, blurry, and sometimes with afterimage tracks or even invisible. The proposed heatmap-based deep learning network is trained to not only recognize the ball image from a single frame but also learn flying patterns from consecutive frames. TrackNet takes images with the size of 640x360 to generate a detection heatmap from several consecutive frames to position the ball and achieve high precision even on public domain videos. The network is evaluated on the video of 2018 Indonesia Open Final - TAI Tzu Ying vs CHEN YuFei. The precision, recall, and F1-measure of TrackNet reach 85.0%, 57.7%, and 68.7%, respectively.
</div>

---

<h3><a href="https://inoliao.github.io/ppTrackNetWebsite/" target="_blank">TrackNet Optimization by Parallel Programming</a></h3>

<div align="justify">
This project exploits the power of parallelism to speedup TrackNet, a deep learning neural network capable of accurately tracking tiny fast-moving objects. An actual 10-minute badminton competition broadcast video is analyzed. 18,243 frames are processed with parallelism mechanism. For Task I: Frame Retrieval from Video, 6-core multiprocessing achieves 2.73 speedup and the total saved time is 344.59 seconds. For Task II: Generating Heatmaps, 6-core multiprocessing achieves as high as 3.97 speedup and the total saved time is 2227.09 seconds. For Task III: TrackNet Model Evaluation, 6-core multiprocessing achieves 1.47 speedup and the total saved time is 17.22 seconds. With parallel programming, both image pre-processing and post-preprocessing processes are significantly accelerated, making the entire object tracking flow much more efficient than before.
</div>

---

<h3><a href="https://inoliao.github.io/nbaWebsite/" target="_blank">NBA Game Prediction System</a></h3>
<div align="justify">
Predicting NBA games is not an easy task. Conventional data analysis and statistic approaches are usually complicated and the accuracy is not high. In this work, a machine learning based method is proposed and the complete design flow is thoroughly introduced and explained. 8 single-stage machine learning models are trained and compared. More complex composite models such as voting mechanism and stacking method are also designed and elaborated. The proposed model reaches 76.8% accuracy on predicting all 2018 NBA playoffs. Furthermore, for the Eastern Conference Final, Western Conference Finals, and Conference Finals, our model achieves an extraordinary prediction accuracy of 85.7%, 71.4%, and 100%, respectively.
</div>

---

<h3><a href="https://github.com/INoLiao/nbaGamePrediction" target="_blank">NBA Stats Crawler</a></h3>
<div align="justify">
In order to predict NBA games, massive NBA stats data must be collected to train the machine learning models. During the NBA regular seasons and playoffs, box scores are updated every single day. Hence, to make data acquisition more efficient and convenient, the NBA Stats Crawler is developed. The crawler scrapes data from the <a href="https://stats.nba.com/teams/boxscores/" target="_blank">official NBA stats website</a> and saves the data as CSV files or in a database. Selenium simulates the humans' behavior of browsing websites and Beautiful Soup is exploited to parse the HTML and retrieve the desired information. With the crawler, both data acquisition and organization are all but a single command on the terminal, preventing enormous and tedious efforts on downloading tons of box scores manually.
</div>
