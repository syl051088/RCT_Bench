Automated, medication-targeted alerts for Acute Kidney Injury – A randomized trial
---

This is a dataset that reflects the data collected as part of a clinical trial known as the "ELAIA-2" trial, which evaluated the effectiveness of automated acute kidney injury alerts for hospitalized individuals exposed to one of three classes of medicaitions of interest.


## Description of the data and file structure

Each row of data represents a single patient enrolled in the ELAIA-2 trial. 

Missing data is expressed as "NaN"

The data columns can be interpreted as follows:

id: a unique identifier for each patient
alert: 1 = randomized to alert group, 0 = randomized to usual care group
hospital: Which of 4 hospitals the patient was admitted at
age_over_90: 1 = patient is 90 years of age or older
age: patient age
sex: 1 = female, 0 = male
icu_at_rand: 1 = in the intensive care unit at randomization
ward_at_rand: 1 = in a hospital ward (ie non-ICU) at randomization
er_at_rand: 1 = in the ER at randomization
num_med: The total number of medications of interest received at randomization (max = 3)
on_acearb: 1 = receiving an RAAS-inhibitor at randomization
on_nsaid: 1 = receiving an NSAID at randomization
on_ppi: 1 = receiving a PPI at randomization
los_since_alert: Length of hospital stay in days (from alert)
death14: 1 = death within 14 days of randomization (discharge alive prior to 14 days assumes alive at 14 days)
dialysis14: 1 = dialysis within 14 days of randomization (discharge alive prior to 14 days assumes no dialysis at 14 days)
aki_progression14: 1= Progression to a higher stage of AKI within 14 days of randomization (discharge alive prior to 14 days assumes no progression at 14 days)
composite_outcome: 1 = any of death14, dialysis14, or aki_progression14
inpatient_mortality: 1 = Death at any time during inpatient stay
inpatient_dialysis: 1 = Dialysis at any time during inpatient stay
progression2: 1 = Progression to stage 2 AKI 
progression3: 1 = progression to stage 3 AKI
acearb_stopped24: 1 = RAASi was stopped within 24 hours of randomization (NaN when patient wasn't receiving at randomization)
nsaid_stopped24: 1 = NSAID was stopped within 24 hours of randomization (NaN when patient wasn't receiving at randomization)
ppi_stopped24: 1 = PPI was stopped within 24 hours of randomization (NaN when patient wasn't receiving at randomization)
no_nsaid_during_aki: 1 = NSAID not given for the duration of AKI (NaN when patient wasn't receiving at randomization)
no_ppi_during_aki: 1 = PPI not given for the duration of AKI (NaN when patient wasn't receiving at randomization)
no_acearb_during_aki: 1 = RAASi not given for the duration of AKI (NaN when patient wasn't receiving at randomization)
time_to_rand: Time (in hours) from admission to randomization
aki_to_rand: Time (in hours) from AKI detection (based on lab values) to randomization:
systolic_max14: The maximum systolic BP (in mmHg) in the 14 days following randomization (safety outcome: missing in those not on RAASi at randomization)
systolic_min14: The minium systolic BP (in mmHg) in the 14 days following randomization (safety outcome: missing in those not on RAASi at randomization)
diastolic_max14: The maximum diastolic BP (in mmHg) in the 14 days following randomization (safety outcome: missing in those not on RAASi at randomization)
diastolic_min14: The minimum diastolic BP (in mmHg) in the 14 days following randomization (safety outcome: missing in those not on RAASi at randomization)
opioid: 1 = Receipt of an opioid within 14 days of randomization (safety outcome: missing in those not on NSAID at randomization)
ventorder: 1 = Mechanical ventilation within 14 days of randomization (safety outcome: missing in those not on RAASi at randomization)
transfuserbc: 1 = Red blood cell transfusion within 14 days of randomization (safety outcome: missing in those not on PPI at randomization)
min_hemoglobin: The minmimum hemoglobin (in g/dL) within 14 days of randomization (safety outcome: missing in those not on PPI at randomization)
duration_of_alert: The time (in days) between the first alert sent and the final alert sent
alert_counter: The number of alerts recived during the study
duration_of_aki: The duration of AKI in days
aki_stage_at_rand: The stage of AKI at randomization
aki_stage14: The maximum AKI stage achieved within 14 days of randomization (not including randomization creatinine. NaN for individuals without a post-randomization creatinine measured).
studytime: The time (in days) since the study was launched at the hospital the patient was admitted to
readmit30: 1 = readmitted within 30 days of discharge
max_pain_score14: The max pain score recorded within 14 days of randomization (NaN = no pain scale recorded)
num_provider: The number of providers who saw an alert for this patient
admit_medical: 1 = patient admitted to a medical service
renalconsult14: 1 = the patient received a formal kidney consult within 14 days of randomization
prior_cs72: 1  = the patient had received a formal kidney consult within the 72 hours prior to randomization
ckd_pmhx: 1 = The medical history included chronic kidney disease (elixhauser system)
chf_elx_pmhx: 1 = The medical history included congestive heart failure (elixhauser system)
pulm_disease_elx_pmhx: 1 = The medical history included pulmonary disease (elixhauser system)
diabetes_elx_pmhx: 1 = The medical history included diabetes (elixhauser system)
htn_elx_pmhx: 1 = The medical history included hypertension (elixhauser system)
malignancy_elx_pmhx: 1 = The medical history included malignancy (elixhauser system)
liverdisease_elx_pmhx: 1 = The medical history included liver disease (elixhauser system)
elx_score_pmhx: The total elixhauser score for the patient (a measure of chronic comorbidity)
creat_at_rand: The creatinine concentration (in mg/dL) at randomization
mincreat48_prior: The lowest creatinine in the 48 hours prior to randomization
mincreat7_prior: The lowest creatinine in the 7 days prior to randomization
maxcreat14_post: The highest creatinine in the 14 days after randomization
mincreat14_post: The lowest creatinine in the 14 days after randomization
admit_creatinine: The first creatinine on hospital admission
baseline_creat: The "baseline" creatinine, as defined by the local minimum creatinine that allowed for the diagnosis of AKI
aniongap_at_rand: The anion gap (in meq/L) at randomization
bicarbonate_at_rand: The serum bicarbonate (in meq/L) at randomization
bun_at_rand: The Blood Urea Nitrogen (in mg/dL) at randomization
chloride_at_rand: The serum chloride (in meq/L) at randomization
egfr_at_admit: The estimated glomerular filtration rate at admission
hemoglobin_at_rand: The hemoglobin concentration (in g/dL) at randomization
plateletcount_at_rand: The platelet count at randomization
potassium_at_rand: The potassium concentration (in meq/L) at randomization
sodium_at_rand: The sodium concentration (in meq/L) at randomization
wbcc_at_rand: The white blood cell count at randomization
systolic_at_rand: The systolic blood pressure at randomization
diastolic_at_rand: The diastolic blood pressure at randomization
pulse_at_rand: The pulse at randomization
resp_at_rand: The respiratory rate at randomization
spo2_at_rand: The oxygen saturation at randomization
temp_at_rand: The body temperature at randomization
sofa_at_rand: The SOFA score (a measure of acute illness) at randomization




## Sharing/Access information

 
Trial Registration: Clinicaltrials.gov NCT02771977. 

Data was derived from the following sources:
  Electronic health record data obtained through the course of usual care. The data was accessed through a series of SQL queries on the Epic "clarity" database. The data was validated on a random subset to ensure accuracy.


