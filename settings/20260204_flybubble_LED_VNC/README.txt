copied from FlyDiscoAnalysis/settings/20210806_flybubble_LED

modified the ctrax results movie params for the 20220414 LED protocol

20220609
changed VNC__barcode to VNC2__barcode in incoming checks

20220913
added jab classifiers

20220914 - make version with jab for VNC (first half of screen)
changed VNC2__barcode to VNC__barcode in incoming checks

20230308 - from 20220913_flybubble_LED_VNC and 20230213_flybubble_LED_VNC2
updating for apt results movie 

20230307
updated the lbl file, same name in apt_params.txt 
Same tracker just updated the slots for tracking and training to work with APT update

20230518
added Alice updated walk jaaba classifier -> scores_walk2.mat

20230623
updated the singularity image pointer for cluster upgrade

20230907
added missing parameter to datalocs 
flytrackerbgstr,movie-bg.mat

20240719
adding params for new stage locomotionmetrics

updates to for LED detection stage change

left alone stats features since those are still in progress

turned on jaabadetect stage

20240906
update gpu queue to gpu_l4_large

20251009
updated from 20240719_flybubble_LED_VNC
add params for locostage via merge with 20251009_flybubble_LED_VNC3
locostage is FORCE for rerunning
fixed gpu queue to be gpu_l4
ground_contact definition is changing - rerun! 

20260204
added param to dataloc for locomotionmetricsperexpfilestr
