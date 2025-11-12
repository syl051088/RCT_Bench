This readme file was generated on 2023-04-12 by Peter Rockers

GENERAL INFORMATION

Title of Dataset: Data from: Evaluation of a community health worker home visit intervention to improve child development in South Africa: A cluster-randomized controlled trial

Author/Co-Principal Investigator Information
Name: Peter C. Rockers
ORCID: 0000-0002-2198-127X
Institution: Boston University
Address: Department of Global Health, Boston University School of Public Health, 801 Massachusetts Avenue, Boston, MA 02119
Email: prockers@bu.edu

Author/Co-Principal Investigator Information
Name: Denise Evans
ORCID: 0000-0003-0698-1228
Institution: Health Economics and Epidemiology Research Office, Wits Health Consortium
Address: 39 Empire Rd, Parktown, Johannesburg, 2193, South Africa
Email: devans@heroza.org

Date of data collection: 2017-09-01 to 2021-06-11

Geographic location of data collection: Limpopo Province, South Africa

Information about funding sources that supported the collection of the data: This study was funded by the South African Medical Research Council (www.samrc.ac.za) 


SHARING/ACCESS INFORMATION

Licenses/restrictions placed on the data: None

Links to publications that cite or use the data: [To be updated]

Links to other publicly accessible locations of the data: None

Links/relationships to ancillary data sets: None

Was data derived from another source? No
If yes, list source(s): 

Recommended citation for this dataset: 

Rockers, Peter C. et al. (2023), Data from: Evaluation of a community health worker home visit intervention to improve child development in South Africa: A cluster-randomized controlled trial, Dryad, Dataset, doi:10.5061/dryad.qnk98sfm2


DATA & FILE OVERVIEW

File List: Rockers et al (2023).csv

Relationship between files, if important: None

Additional related data collected that was not included in the current data package: None

Are there multiple versions of the dataset? No
If yes, name of file(s) that was updated: 
Why was the file updated? 
When was the file updated? 


METHODOLOGICAL INFORMATION

Description of methods used for collection/generation of data:

Data are from a cluster-randomized controlled trial conducted in Zambia. Household survey data were collected from 1,095 caregiver-child dyads residing in 51 clusters at baseline (2017) and from 764 dyads remaining enrolled at endline (2021). At endline, child height was measured and child development was assessed using the Malawi Developmental Assessment Tool (MDAT). EEG and eye-tracking assessments were conducted among a subset of children at a centrally located laboratory at endline and at two interim time points. In total, 316 dyads attended the first lab visit, 316 dyads the second lab visit, and 284 dyads the third lab visit. More detail on data collection is provided in Rockers et al. (2023).

Methods for processing the data:

Height-for-age z-scores were constructed from height data using the WHO Child Growth Standards. Stunting was defined as HAZ < -2. Child development scores in the domains of gross motor, fine motor, language, and social development, measured using the Malawi Developmental Assessment Tool (MDAT). Raw scores of successfully completed items were summed within each domain and then converted to z-scores using the MDAT scoring application. EEG data were first filtered using Net Station software with a 50 Hz notch filter to remove electrical noise and 70 Hz low pass filter. The data were then pre-processed in MATLAB using the Harvard Automated Processing Pipeline for EEG. Data from the first assessment wave were segmented into two-second epochs, while data from the second and third waves were segmented into one-second epochs. A wavelet-enhanced independent components analysis approach was used to correct for artifact while retaining the entire length of the data file. Bad channels were replaced using spherical spline interpolation, and data were re-referenced to the average reference. Following independent components analysis, observations with more than 15% bad channels, more than five interpolated channels, fewer than 40 one-second epochs of usable data out of a possible 360 epochs, or median artifact probability greater than 33% for retained independent components were excluded from the analysis for quality reasons. EEG power was then computed in MATLAB using the Batch Electroencephalography Automated Processing Platform. Channel measures of absolute gamma power per Hz (30-48 Hz) and total power were averaged across the entire brain for each assessment at each wave and then log-transformed. A measure of relative gamma power was generated for each assessment at each wave by dividing average gamma power across the entire brain by average total power across the entire brain. SRT estimates were extracted from raw eye-tracking data by an automated script that: applies a median-filter to remove abrupt spikes; merges the xy-coordinates for the two eyes by averaging or by using the data of one valid eye; and verifies that the recorded saccade reflects a valid gaze shift from the area of the previous saccade target to the area of the new target within the expected time window and is not contaminated by missing or noisy data. Saccades passing the pre-set validity criteria (10 or more valid saccades) were used to calculate mean SRT.

Instrument- or software-specific information needed to interpret the data: The data are in CSV format, which can be imported by most statistical sofware programs

Standards and calibration information, if appropriate: None

Environmental/experimental conditions: A home-visit intervention in which community health workers were provided with and trained on a job aid that included content on child health, nutrition, developmental milestones, and encouragement to engage in developmentally appropriate play-based activities.

Describe any quality-assurance procedures performed on the data: None

People involved with sample collection, processing, analysis and/or submission: Data were collecting by a team based at the Health Economics and Epidemiology Research Office, Wits Health Consortium


DATA-SPECIFIC INFORMATION FOR: Rockers et al (2023).csv

Number of variables: 63

Number of cases/rows: 1,095

Variable List:

id			Unique participant identifier
clusterid		Unique cluster identifier
subdistrict		0: Greater Giyani; 1: Greater Tzaneen
lab1_month		Month of wave 1 lab visit
lab1_year		Year of wave 1 lab visit
lab2_month		Month of wave 2 lab visit
lab2_year		Year of wave 2 lab visit
lab3_month		Month of wave 3 lab visit
lab3_year		Year of wave 3 lab visit
el_month		Month of endline assessment
el_year			Year of endline assessment
mdat_lab		0: MDAT assessed at home; 1: MDAT assessed at lab
lab1_room_eeg		Room/unit number of wave 1 EEG assessment
lab1_room_et		Room/unit number of wave 1 eye-tracking assessment
lab2_room_eeg		Room/unit number of wave 2 EEG assessment
lab2_room_et		Room/unit number of wave 2 eye-tracking assessment
lab3_room_eeg		Room/unit number of wave 3 EEG assessment
lab3_room_et		Room/unit number of wave 3 eye-tracking assessment
treatment		0: control; 1: treatment
lab1_age		1: Child 6-8 months old at wave 1 lab visit; 2: Child 9-11 months old at wave 1 lab visit
lab2_age		1: Child 15-16 months old at wave 2 lab visit; 2: Child 17-18 months old at wave 2 lab visit
lab3_age		1: Child 30-35 months old at wave 3 lab visit; 2: Child 36-41 months old at wave 3 lab visit
el_age			1: Child 30-35 months old at endline assessment; 2: Child 36-43 months old at endline assessment
el_assessor		Unique assessor identifier at endline
bl_caregiver_age	Caregiver age (years) at baseline (1: 18-25; 2: 26-30; 3: 31-35; 4: 36-40; 5: 41-45; 6: 46-50; 7: 51+)
bl_caregiver_matric	0: Caregiver did not receive matriculation certificate (did not complete gradde 12); 1: Caregiver received matriculation certificate (completed grade 12)
bl_wealth_z		Household wealth index z-score at baseline
bl_wealth_q		Household wealth index quantile at baseline (1: poorest; 5: least poor)
bl_childgrant		0: Household did not receive Child Grant at baseline; 1: Household received Child Grant at baseline
siblings		0: No siblings at baseline; 1: 1+ siblings at baseline
el_haz			Height-for-age z-score at endline
el_stunted		0: Not stunted at endline; 1: Stunted at endline
el_mdat_gm_z		MDAT gross motor z-score at endline
el_mdat_fm_z		MDAT fine motor z-score at endline
el_mdat_lang_z		MDAT language z-score at endline
el_mdat_soc_z		MDAT socioemotional z-score at endline
el_dd			Diet diversity score at endline
el_mics			MICS score at endline
lab1_srt		Saccadic reaction time at wave 1 (ms)
lab2_srt		Saccadic reaction time at wave 2 (ms)
lab3_srt		Saccadic reaction time at wave 3 (ms)
lab1_gamma		Absolute gamma power at wave 1 (ln[µV2/Hz])
lab2_gamma		Absolute gamma power at wave 2 (ln[µV2/Hz])
lab3_gamma		Absolute gamma power at wave 3 (ln[µV2/Hz])
lab1_total		Absolute total power at wave 1 (ln[µV2/Hz])
lab2_total		Absolute total power at wave 2 (ln[µV2/Hz])
lab3_total		Absolute total power at wave 3 (ln[µV2/Hz])
lab1_relgamma		Relative gamma power at wave 1
lab2_relgamma		Relative gamma power at wave 2
lab3_relgamma		Relative gamma power at wave 3
lab1_srt_trials		Number of valid saccade trials at wave 1
lab2_srt_trials		Number of valid saccade trials at wave 2
lab3_srt_trials		Number of valid saccade trials at wave 3
lab1_channels		Number of EEG channels with usable data at wave 1
lab2_channels		Number of EEG channels with usable data at wave 2
lab3_channels		Number of EEG channels with usable data at wave 3
lab1_src		EEG SRC at wave 1 (measure of data quality)
lab2_src		EEG SRC at wave 2 (measure of data quality)
lab3_src		EEG SRC at wave 3 (measure of data quality)
cluster_facilities	Number of facilities in cluster
cluster_wbots		Number of ward-based outreach teams in cluster
cluster_chws		Number of community health workers in cluster
cluster_phcu5		Number of under-5 primary health care visits per month at facilities in cluster
cluster_chwage		Average age of community health workers in cluster
cluster_chweduc		Average years of education of community health workers in cluster
cluster_chwworkyr	Average years in the position for community health workers in cluster
chw_1m			0: Intervention CHW did not make home visit in previous month; 1: Intervention CHW made home visit in previous month
chw_3m			0: Intervention CHW did not make home visit in previous 3 months; 1: Intervention CHW made home visit in previous 3 months
chw_ecd			0: During recent visit CHW did not counsel caregiver on child development content of the job aid; 1: During recent visit CHW counselled caregiver on child development content of the job aid

Missing data codes: -99 for all numeric variables

Specialized formats or other abbreviations used: None