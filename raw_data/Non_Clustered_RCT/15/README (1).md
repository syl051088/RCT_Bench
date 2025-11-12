# Data from: The effect of Snoezelen intervention on problem behaviors in children with cerebral palsy: A randomized controlled trial

[https://doi.org/10.5061/dryad.9cnp5hqtv](https://doi.org/10.5061/dryad.9cnp5hqtv)

## Description of the data and file structure

This dataset was collected as part of a randomized controlled trial to evaluate the effect of **Snoezelen intervention** on **problem behaviors** in children with cerebral palsy (CP). The trial involved 28 participants aged 2 to 5 years, divided into an experimental group receiving the Snoezelen intervention and a control group receiving standard care. Data was collected over a 4-week period, with the experimental group receiving Snoezelen sessions three times a week. **Problem behaviors** and emotional changes were assessed using the **Child Behavior Checklist (CBCL)** and the **Korean Parenting Stress Index (K-PSI)** before and after the intervention.

### Files and variables

### Case\_Report\_Form(250222).csv

This file contains **demographic data and behavioral assessment scores (CBCL, K-PSI) before and after the intervention.**

### **Variables in the dataset:**

* **participant_id**: Unique identifier for each participant
* **side**: A categorical variable indicating the affected side of the body (1 = bilateral, 2 = unilateral) 
* **type**: A categorical variable describing the type of cerebral palsy (1 = spastic, 2 = dyskinetic, 3 = ataxic, 4 = mixed)
* **GMFCS_level**: Gross Motor Function Classification System level (`1` to `5`)
* **Group:** A categorical variable indicating the group assignment of participants (1 = Experimental group (A), 2 = Control group (B))
* **CBCL_Total_1**: CBCL total score **before** the intervention(range: 0-100)
* **Inter_1**: Internalizing score (CBCL) **before** the intervention
* **Exter_1**: Externalizing score (CBCL) **before** the intervention
* **Emo.R._1**: Emotional reactivity score **before** the intervention
* **Anx./Dep._1**: Anxiety/Depression score **before** the intervention
* **Somatic_1**: Somatic complaints score **before** the intervention
* **Withd._1**: Withdrawal behavior score **before** the intervention
* **Sleep_1**: Sleep problems score **before** the intervention
* **Attention_1**: Attention problems score **before** the intervention
* **Aggressive_1**: Aggressive behavior score **before** the intervention
* **Others_1**: Other behavioral issues score **before** the intervention
* **Child_1**: Child-reported stress score **before** the intervention
* **Parent_1**: Parent-reported stress score **before** the intervention
* **PSI_Total_1**: Parenting Stress Index (PSI) total score **before** the intervention(range: 0-100)
* **CBCL_Total_2**: CBCL total score **after** the intervention
* **Inter_2**: Internalizing score (CBCL) **after** the intervention
* **Exter_2**: Externalizing score (CBCL) **after** the intervention
* **Emo.R._2**: Emotional reactivity score **after** the intervention
* **Anx./Dep._2**: Anxiety/Depression score **after** the intervention
* **Somatic_2**: Somatic complaints score **after** the intervention
* **Withd._2**: Withdrawal behavior score **after** the intervention
* **Sleep_2**: Sleep problems score **after** the intervention
* **Attention_2**: Attention problems score **after** the intervention
* **Aggressive_2**: Aggressive behavior score **after** the intervention
* **Others_2**: Other behavioral issues score **after** the intervention
* **Child_2**: Child-reported stress score **after** the intervention
* **Parent_2**: Parent-reported stress score **after** the intervention
* **PSI_Total_2**: Parenting Stress Index (PSI) total score **after** the intervention

### Missing Values:

* Missing values are indicated with **"NA"** in all data files.

## Code/software

**Software**: The data was analyzed using IBM SPSS Statistics. This software was used to perform various statistical tests, including descriptive statistics, Spearman's rank correlation, and non-parametric tests such as the Mann-Whitney U test and Wilcoxon Signed-Rank test.

**Code/Scripts**: No custom code or scripts were used, as the analysis was conducted using built-in functionalities of IBM SPSS.

**Workflow**: The dataset, provided in CSV format, was imported into IBM SPSS for analysis. Descriptive statistics were first calculated to summarize demographic information and behavior changes. The Spearman's correlation test was used to assess relationships between GMFCS levels and emotional reactivity changes, and non-parametric tests were performed to compare the experimental and control groups' pre- and post-intervention results.

## Access information

No external datasets were used in this study. All data were collected as part of the current research project.
