# Data from a randomized controlled trial: Comparison between high-flow nasal cannula (HFNC) therapy and noninvasive ventilation (NIV) in children with acute respiratory failure by bronchiolitis

This dataset contains information on each patient randomized to the study. The first row describes the variables registered. From the second row onwards, each of them represents the variables of a unique patient that include indirect data, values ​​found during the period on high-flow or NIV and also during hospitalization that were used for statistical analysis between the groups.

*Column legends:*

Plot_ID: identifier for study plot

Gn: gender (male = 0, female = 1)

Ag: age ranges in months (e.g. 7 was replaced with 6-8)

We: weight ranges in kilograms (e.g. 7,5 was replaced with 6-8)

PW: previous weezing (n = no, y = yes)

PRH: previous respiratory hospitalization (n = no, y = yes)

Em: protocol finalization at emergency department (n = no, y = yes)

Trn: external transfer after intubation (n = no, y = yes)

Gr: group randomized (NIV = noninvasive ventilation, HFNC = high-flow nasal cannula)

VP: viral panel (RSV = respiratory syncytial virus, Bo = bocavirus, SC = seasonal coronavirus, Pa = parainfluenza, Ad = adenovirus, Me = metapneumovirus, RE = rhino/enterovirus, NA = sample not available)

It: intubation

TD: HFNC/NIV duration in hours

\_0 (e.g. HR_0) = heart rate at protocol initiation

\_2 (e.g. HR_2) = heart rate after 2h of protocol initiation

\_6 (e.g. HR_6) = heart rate after 6h of protocol initiation

\_12 (e.g. HR_12) = heart rate after 12h of protocol initiation

\_24 (e.g. HR_24) = heart rate after 24h of protocol initiation

\_48 (e.g. HR_48) = heart rate after 48h of protocol initiation

\_72 (e.g. HR_72) = heart rate after 72h of protocol initiation

\_96 (e.g. HR_96) = heart rate after 96h of protocol initiation

HR: heart rate

RR: respiratory rate

SpO2: peripheral oxygen saturation

WD: Wood-Downes-Férres score

FiO2: fraction of inspired oxygen

L/min: liters per minute (HFNC)

IPAP: inspiratory positive airway pressure (NIV)

EPAP: expiratory positive airway pressure (NIV)

SDu: sedation duration (in days)

ETu: enteral tube duration (in days)

NPI: nasal pressure injury (n = no, y = yes)

PLOS: PICU length of stay ranges in days (e.g. 7 was replaced with 6-8)

HLOS: hospital length of stay ranges in days (e.g. 7 was replaced with 6-8)

MV: mechanical ventilation duration (in days)

ATB: antibiotic requirement (n = no, y = yes)

PIM: Pediatric Index of Mortality

De: death (n = no, y = yes)

pf: protocol finalized

md: missing data

nc: not calculated

negative: viral panel with no virus identified

After data curation, some adjustments were done to facilitate dataset comprehension and to respect data sharing for human subjects:

1\) Blank spaces have been eliminated

2\) The identification of each column has been adjusted according to the standards and described in detail in the README

3\) In the viral panel column = the "+" symbol has been eliminated and the results have been separated by commas

4\) For protocols that have already been finalized, the letter "x" has been replaced by "pf" to facilitate understanding

5\) Column “Age”, "We", PLOS and HLOS: the specific age (in months), weight (in kilograms), PICU length of stay (in days) and hospital length of stay (in days) were replaced with the respectively ranges (e.g. 6 was replaced with 0-5)

6\) For gender, male (“m”) and female (“f”) were replaced by 0 (male) and 1 (female).

7\) Empty cell was filled with "nc" and the number "10" was transferred to the appropriate column Z

8\) "sr" was has been replaced by "md" (missing data)