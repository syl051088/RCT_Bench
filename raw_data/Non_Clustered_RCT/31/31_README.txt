Data and R scripts for the following publication:

Cowling BJ, Lim WW, Perera RAPM, Fang VJ, Leung GM, Peiris JSM, Tchetgen Tchetgen EJ. Influenza hemagglutination-inhibition antibody titer as a mediator of vaccine-induced protection for influenza B. (submitted paper)

+-----------------+
|  List of files  |
+-----------------+

1. [kid_all.csv] This data file contains all data information.
Definition of column headings >>>
hhID: ID of study participants
age: age of participants, in years
intervention: the vaccination group assigned to each participant (1-TIV, 2-Placebo)
vaccine: the vaccination status for each participant (1-vaccinated, 0-unvaccinated/placebo)
vaccine.date: date of vaccination
postvax.date: date of blood collection for estimation of post-vaccination titers
prevax.B.Brisbane: pre-vaccination titers
postvax.B.Brisbane: post-vaccination titers
surv_time: survival time/time from reference date to time of event (flu infection or censoring/end of study)
flu: 1 - flu infection confirmed by RT-PCR; 0 - no flu infection detected throughout study, censored at the end of study

2. [Mediation_functions.r] R syntax including functions needed in the analyses.

3. [Mediation_analysis.r] R syntax for mediation analysis results.

4. [Results_and_figures.r] R syntax to reproduce descriptive results and Figure 2.

