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

20240910
merged 20240908_flybubble_centralcomplex and 20210520_flybubblered_nochr_flytracker to make flydisco settings directory for reprocessing

20240913
change gpu queue to gpu_l4

20240917
add JAABA social touch classifier that has only built in apt features - to precompute those

20250113
added nottracking.jab file - uses APT features so increase storage space
removed /groups/branson/home/robiea/Projects_data/JAABA/ProjectFiles_jab/FlyDisco/flsocialtouch_v6.jab

20260422
forked from 20250113_flybubblered_nochr_flytracker for screen_type non_olympiad_branson_MSA
(Bill Lemon MSA mutant flies, doChR=0, RGG rig, 600s recording)
VNC3 ports below are all from 20260326_flybubble_LED_VNC3
- JAABA_classifier_params.txt: replaced flsocialtouch_v6.jab + nottracking_aptv4.jab with nottracking_aptv7p1.jab
- analysis-protocol-parameters.txt: matched VNC3 stage ordering; added doaddpflies,off; removed dotrackwings;
  added dolocomotionmetrics,off; added docleanup,force
- added cleanup_params.txt, blacklist_globs.txt, whitelist_globs.txt (from VNC3)
- added jaaba_detect_params.txt (from VNC3, fastcomputepffs,1)
- dataloc_params.txt: added cleanupparamsfilestr,cleanup_params.txt
- automatic_checks_incoming_params.txt: min_movie_length_seconds 295 -> 595 (600s recording);
  desired_files barcode cx__BARCODE.csv -> MSA__BARCODE.csv
- registration_params.txt: doTemporalTruncation 0 -> 600 (truncate black frames at end of movie);
  simplified bowlMarkerType to single CircleTemplateLarge.png
