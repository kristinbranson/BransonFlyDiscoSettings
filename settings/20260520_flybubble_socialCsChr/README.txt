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

20240908 
merged 20240507_flybubble_LED_VNC3 and 20150915_flybubble_centralcomplex to make flydisco settings directory for reprocessing

20240912
updated npad in indicator to get envelop instead of the following pulses. found new value analytically by testing with distinct_pulse_count_from_single_channel_protocol

20240913
changed queue to gpu_l4

20250113
added nottracking.jab file - uses APT features so increase storage space

20260520
copied from FlyDiscoAnalysis/settings/20250113_flybubble_socialCsChr
new settings dir for socialCsChr experiments collected starting the week of 2026-05-25
current_non_olympiad_branson_socialCsChr repointed here from 20250113_flybubble_socialCsChr

added locostage files/params (locostage itself stays OFF in this protocol):
  locomotionmetrics_params.txt: copied from 20260518_flybubble_LED_reprocessregistrationbug_VNC
    (includes onfloor filtering params: walking/onceiling/nottracking score files, frac_onfloor_threshold)
  dataloc_params.txt: added three entries after aptresultsmovieparamsfilestr:
    locomotionmetricsparamsfilestr,locomotionmetrics_params.txt
    locomotionmetricsswingstanceboutstatsfilestr,locomotionmetrics_swingstancebouts.mat
    locomotionmetricsperexpfilestr,locostatsperexp_onfloor.mat
  analysis-protocol-parameters.txt: inserted dolocomotionmetrics,off after dojaabadetect

JAABA params updated to match VNC:
  JAABA_classifier_params.txt: nottracking classifier
    FlyBubble/nottracking_aptv4.jab -> FlyDisco/nottracking_aptv7p1.jab
  jaaba_detect_params.txt: new file with fastcomputepffs,1
    (dataloc_params.txt already referenced this file)

added cleanup stage (matches VNC 20260326):
  cleanup_params.txt, blacklist_globs.txt, whitelist_globs.txt: copied from
    20260518_flybubble_LED_reprocessregistrationbug_VNC
  dataloc_params.txt: added cleanupparamsfilestr,cleanup_params.txt
  analysis-protocol-parameters.txt: appended docleanup,force
  
20260601
fixed markertemplate - claude kept old style per plate which caused all experiments to fail. 
changed exceptable load time to 35 seconds

20260601
the template for the marker was missing, copied over from /settings/20260422_flybubble_MSA_nochr/CircleTemplateLarge.png
