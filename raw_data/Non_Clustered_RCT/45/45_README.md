# Price discounts on low energy dense foods on food intake and health status

[https://doi.org/10.5061/dryad.np5hqbzz9](https://doi.org/10.5061/dryad.np5hqbzz9)

Contains all data for statisical analysis for participants who completed up to the midpoint of the intervention period.
**Research objective**: To test the effects of multi-level supermarket discounts on fruit and vegetable (F&V) and non-caloric beverage consumption, as well as health outcomes.
**Intervention**: Economic intervention of multilevel (30, 15, 0%) price discounts on fruit, vegetable, and non-caloric beverage intake. These price discounts were implemented in an NYC grocery store chain at the point-of-purchase to assess the effect of the intervention on fruit, vegetable, and non-caloric beverage intake. Discounts were administered via store loyalty cards. Store cards were used each time the participant shopped for the duration of the study.
**Study Design**: A randomized controlled trial of adults grocery shoppers with overweight/obese status in NYC.
**Study Timeline:**

*   Week 0, visit 1: Baseline period.
*   Week 8, visit 2: Start of the intervention period
*   Week 24, visit 3: Intervention midpoint

Procedure: **Baseline period**: at week 0 the first study visit occurred. Clinical measurements (body weight, waist circumferences, BMI, body composition, blood pressure, and blood draw) were taken. Questionnaires such as an income questionnaire, and behavioral checklist (to assess study protocol adherence and to monitor lifestyle changes that occur between visits) were administered. A training 24-h dietary recall was administered to prepare participants for this dietary assessment during the study. Participants were given a new Foodtown loyalty card to use. About a month before the intervention period, interviewer-led 24-hour dietary recalls were administered to participants. **Intervention period**: at week 8 the intervention period began. Study visit 2 occurred similar to visit 1, with the exception of the income questionnaire and training 24-hr recall. Participants were informed that the current study visits mark the beginning of the intervention period. They were given a summary list of foods and drinks that were discounted. Randomization occurred after the study visit. Participants were randomized by sex and store into one of three intervention groups to receive a 30%, 15% or 0% (control) discount on applicable fruits, vegetables, and non-caloric beverages. Participants were informed which group they were randomized to. About a month before the midpoint (week 24) interviewer-led dietary recalls were administered. At week 24, study visit 3 occurred. This visit was similar to visit 1, with the exception of the income questionnaire and training 24-h recall.
**Measures:** **Dietary intake**: 24-h dietary recalls, interviewer-led using the multiple pass method. This assessment was used to assess dietary intake for 2-weekdays and 1-weekend day. Intake reported by participants were entered into Foodwork18 to generate a nutrient reports. From the report, kilocalories from food, grams of food, energy density (ED), and grams of fruit, vegetables, and non-caloric beverages, as well as other food group/patterns were calculated. **Clinical measurements** are as follows: body weight (lbs and kg), bmi (kg/m2), and waist circumference (inches), body composition using TANITA BIA (gives % body fat), blood pressure in mm/Hg, blood analytes: fasting glucose (acute measure of blood sugar concentration) and HbA1c (long-term measure of blood glucose concentration, about 2-3 months), Lipid panel: Total cholesterol, HDL-c, LDL-c, triglyerides.
Questionnaires: - **Income:** household income range **Behavioral checklist:** to assess study protocol adherence and to monitor lifestyle changes that occur between visits.

## Description of the data and file structure

Prefixes

| Prefix                                                           | Data type                                | Description                                                                                |
| :--------------------------------------------------------------- | :--------------------------------------- | :----------------------------------------------------------------------------------------- |
| Time data collected for clinical measurements and questionnaires |                                          |                                                                                            |
| pre                                                              | clinical measurements and questionnaires | collected at the start of the intervention period (V2)                                     |
| post                                                             | clinical measurements and questionnaires | collected at the intervention midpoint (V3)                                                |
| Time data collected for dietary recalls                          |                                          |                                                                                            |
| pre                                                              | dietary assessment                       | collected during the first half of the intervention period (\~1 week before (midpoint) V3) |
| post                                                             | dietary assessment                       | collected during the last half of the intervention period(\~1 week before V4)              |

Variables

| Variable  name | Data type          | Description                                                                                                                                                             |
| :------------- | :----------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| discount       | PPT Info           | intervention group assignment                                                                                                                                           |
| income\_group  | PPT Info           | income group as 2 levels: Less than 50K, Greater than 50K                                                                                                               |
| covid\_present | PPT Info           | Whether or not the participants data collected after COVID                                                                                                              |
| store          | PPT Info           | Main store                                                                                                                                                              |
| store\_type    | PPT Info           | Store type: big, small , or other                                                                                                                                       |
| length         | PPT Info           | number of days between study visits                                                                                                                                     |
| shopping       | PPT Info           | % shopping at store reported by the ppt at study visit                                                                                                                  |
| weight         | Clinical data      | avg weight in lbs                                                                                                                                                       |
| kg             | Clinical data      | avg body weight in kg calculated from weight                                                                                                                            |
| bmi            | Clinical data      | kg/m2                                                                                                                                                                   |
| waist          | Clinical data      | avg wasit circumference in inches                                                                                                                                       |
| fat            | Clinical data      | % fat mass                                                                                                                                                              |
| percentfat     | Clinical data      | the actual number for % fat mass                                                                                                                                        |
| fm             | Clinical data      | fat mass in kg. calculated by multiplying the percent fat (fraction) by   body mass (in kg)                                                                             |
| ffm            | Clinical data      | fat free mass in kg. calculated by subtracting the body mass minus the   fat mass                                                                                       |
| sysbp          | Clinical data      | avg systolic BP (mm/Hg)                                                                                                                                                 |
| diabp          | Clinical data      | avg diastolic BP (mm/Hg)                                                                                                                                                |
| gluc           | Clinical data      | fasting glucose                                                                                                                                                         |
| hba1c          | Clinical data      | %                                                                                                                                                                       |
| tc             | Clinical data      | total cholesterol                                                                                                                                                       |
| hdl            | Clinical data      | HDL-cholesterol                                                                                                                                                         |
| ldl            | Clinical data      | LDL-cholesterol                                                                                                                                                         |
| tg             | Clinical data      | triglyerides                                                                                                                                                            |
| kcalfood       | dietary assessment | total kcal from foods, Reported during 24h recall.                                                                                                                      |
| gramsfood      | dietary assessment | total grams of food, Reported during 24h recall.                                                                                                                        |
| ed             | dietary assessment | kcal from foods over the gram weight of foods Reported during 24h recall.                                                                                               |
| fruit          | dietary assessment | fruits, includes foods commonly known/consumed as fruits, excludes dried   fruits, fruit juice, and fruits packaged in syrup Reported during 24h recall.                |
| veg            | dietary assessment | vegetables, includes foods commonly known/consumed as vegetables,   excludes vegetables packaged with non-vegetables (e.g., creamed corn)   Reported during 24h recall. |
| fv             | dietary assessment | total of fruits and vegetables Reported during 24h recall.                                                                                                              |
| soda           | dietary assessment | soda, includes soft drinks, colas, sweetened with sugar Reported during   24h recall.                                                                                   |
| juice          | dietary assessment | juice sweetened with sugar Reported during 24h recall.                                                                                                                  |
| icedtea        | dietary assessment | presweetened iced tea Reported during 24h recall.                                                                                                                       |
| ssb            | dietary assessment | sum of soda, juice, and iced tea Reported during 24h recall.                                                                                                            |
| bottledwater   | dietary assessment | bottle water intake. Reported during 24h recall                                                                                                                         |
| seltzerwater   | dietary assessment | zero cal seltzer water/carbonated water intake. Reported during 24h   recall.                                                                                           |
| dietsoda       | dietary assessment | zero-calorie soft drinks and colas Reported during 24h recall.                                                                                                          |
| noncalbev      | dietary assessment | sum of diet soda, seltzer, and bottled water. Reported during 24h recall.                                                                                               |
| alcohol        | dietary assessment | alcoholic beverages (all types) Reported during 24h recall.                                                                                                             |
| totalsnack     | dietary assessment | total high calorie snack foods. This is the sum of sweet and salty snack   foods Reported during 24h recall.                                                            |
| salty          | dietary assessment | salty snack foods (i.e., chips, nuts, seeds, popcorn, crackers)                                                                                                         |
| sweet          | dietary assessment | sweety snack foods (i.e., chocolate, cake, candy, ice cream, etc.)                                                                                                      |
| fats           | dietary assessment | oils and fats (butter, lard, etc.) Reported during 24h recall.                                                                                                          |
| hed            | dietary assessment | solid foods wtih EDs at or above 3.5 kcal/g Reported during 24h recall.                                                                                                 |
| led            | dietary assessment | solid foods wtih EDs at or below 1.2 kcal/g Reported during 24h recall.                                                                                                 |

