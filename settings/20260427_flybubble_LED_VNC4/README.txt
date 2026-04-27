copied from FlyDiscoAnalysis/settings/20210806_flybubble_LED

modified the ctrax results movie params for the 20220414 LED protocol

20220609
changed VNC_barcode to VNC2__barcode in incoming checks

20220913
added jab classifiers

202201005
added parameters for APT tracking

20230213 from - 20220913_flybubble_LED_VNC2
adding parameters for apt results movie

20230307
updated the lbl file, same name in apt_params.txt 
Same tracker just updated the slots for tracking and training to work with APT update

20230518
added Alice updated walk jaaba classifier -> scores_walk2.mat

20230622
updated the singularity image pointer for cluster upgrade

20230907
added missing parameter to datalocs 
flytrackerbgstr,movie-bg.mat

20240906
update gpu queue to gpu_l4_large

20240913
change gpu queue to gpu_l4

20241203
add locomotion stage

20251009 
add locomotion stage params

20260204
add param to dataloc for locomotionmetricsperexpfilestr

20260326
added jaaba_detect_params.txt with fastcomputepffs,1
added nottracking_aptv7_nowindowdata.jab to JAABA_classifier_params.txt
added cleanup stage (docleanup,force) to delete perframe/apt*.mat files
added cleanup_params.txt, blacklist_globs.txt, whitelist_globs.txt
added cleanupparamsfilestr to dataloc_params.txt
added onfloor filtering params to locomotionmetrics_params.txt: walking_score_file, onceiling_score_file, nottracking_score_file, frac_onfloor_threshold
changed locomotionmetricsperexpfilestr to locostatsperexp_onfloor.mat in dataloc_params.txt
updated nottracking classifier from nottracking_aptv7_nowindowdata.jab to nottracking_aptv7p1.jab

20260427
forked from 20260326_flybubble_LED_VNC3 for VNC4 screen
(VNC4: followup experiments with known phenotypes)
- automatic_checks_incoming_params.txt: desired_files barcode VNC3__BARCODE.csv -> VNC4__BARCODE.csv
