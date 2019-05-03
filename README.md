# PsychHacks2019
Dataset available for UofT PsychHacks2019

pupil_data.csv.zip: Contains sample report extracted from Eyelink (R) 1000 at frequency of 20Hz for 48 participants.

Study design:
Participants view face images for 6 blocks and perform a remember-know-new (RKN) recognition task in the last 3 blocks.

Study blocks 1-2 (60 trials in each block): Exposure-I (60 face images presented twice)<br/>
Study blocks 3-5 (40 trials in each block): Indirect Test (60 face images from Exposure-I presented for the 3rd time and 60 new face images presented once)<br/>
Study block 6 (60 trials): Exposure-II (60 face images that were presented for the first time in Block 3-5, presented once again)<br/>

Test blocks 1-3 (40 trials in each block): Direct Test (60 face images from Exposure-II that were presented twice before and 60 new face images presented once)<br/>

Variables:<br/>
```
"recording_session_label": subject number </br>
"trial_index": trial number (1:420)<br/>
"right_fix_index": fixation index<br/>
"right_in_blink": blink (1) or not (0)<br/>
"right_in_saccade": saccade (1) or not (0)<br/>
"right_pupil_size": pupil size<br/>
"right_saccade_index": saccade index<br/>
"sample_index": sample number (ms)<br/>
"timestamp": timestamp (generated by Eyelink)<br/>
"trial_start_time": timestamp when the trial started (generated by Eyelink)<br/>
"study_end": end time of study trial (only for study blocks 1-6, i.e., trials 1-300; NA otherwise)<br/>
"study_start": start time of study trial (only for study blocks 1-6, i.e., trials 1-300; NA otherwise)<br/>
"test_end": end time of test trial (only for test blocks 1-3, i.e., trials 301-420; NA otherwise)<br/>
"test_start": start time of test trial (only for test blocks 1-3, i.e., trials 301-420; NA otherwise)<br/>
"test_response": response on the test trial -- 106 ("remember"), 107 ("know"), 108 ("new")<br/>
"test_rt": response time on the test trial (ms)<br/>
"study_block": study block number (1:6)<br/>
"study_image": image label of the study trial (JPG)<br/>
"study_old_num": whether the image was old or new (only for study blocks 3-5)<br/>
"study_trial": trial number within block (1:40 for study blocks 3-5; 1:60 for study blocks 1,2,6)<br/>
"test_block": test block number (1:3)<br/>
"test_image": image label of the test trial (JPG)<br/>
"test_old_num": whether the image was old or new (only for test blocks)<br/>
"test_trial": trial number within block (1:40)<br/>
"sample_blink_outlier": outlier based on whether the eye is in a fixation (0) or not (1)<br/>
"pupil_after": whether the sample index is higher (1) or lower (0) than response time<br/>
"pupil_before": whether the sample index is higher (0) or lower (1) than response time<br/>
"pupil_mean_after": mean pupil size for sample indices higher than response time<br/>
"pupil_mean_before": mean pupil size for sample indices lower than response time<br/>
"pupil_last": whether the sample index is in the first 1500 ms (0) or the last 1500 ms (1) (out of the 3000ms trial)<br/>
"pupil_first": whether the sample index is in the first 1500 ms (1) or the last 1500 ms (0) (out of the 3000ms trial)<br/>
"pupil_mean_last": mean pupil size for sample indices higher than 1500 ms<br/>
"pupil_mean_first": mean pupil size for sample indices lower than 1500 ms<br/>
```
