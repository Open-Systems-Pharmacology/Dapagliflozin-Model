### 2.2.1	In vitro / physico-chemical Data

A literature search was performed to collect available information on physiochemical properties of dapagliflozin. The obtained information from literature is summarized in the table below. 

| **Parameter**   | **Unit** | **Value** | Source                                           | **Description**                                 |
| :-------------- | -------- | --------- | ------------------------------------------------ | ----------------------------------------------- |
| MW              | g/mol    | 408.873   | [DrugBank DB06292](# 5 References)               | Molecular weight                                |
| pK<sub>a</sub>  |          | 12.57     | [DrugBank DB06292](# 5 References)               | Acid dissociation constant                      |
| Solubility (pH) | mg/mL    | 0.173 (7) | [DrugBank DB06292](# 5 References)               | Aqueous Solubility                              |
| logP            |          | 2.7       | [DrugBank DB06292](#5 References) (experimental) | Partition coefficient between octanol and water |
| fu              | %        | 9         | [Obermeier 2009](#5 References)                  | Fraction unbound in plasma                      |
| B/P ratio       |          | 0.88      | [Obermeier 2009](#5 References)                  | Blood to plasma ratio                           |

### 2.2.2	Clinical Data

A literature search was performed to collect available clinical data on dapagliflozin in healthy adults.

#### 2.2.2.1	Model Building

The following studies were used for model building (training data):

| Publication                                                  | Arm / Treatment / Information used for model building        |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [Boulton 2013](#5 References)                                | 14C-dapagliflozin intravenous and<br />Dapagliflozin oral administration |
| [DeFronzo 2013](#5 References)                               | Healthy subjects with a single oral dose of 10 mg            |
| [Imamura 2013](#5 References)                                | Control phase with a single oral dose of 10 mg               |
| [Kasichayanula 2008](#5 References)                          | Mass balance information                                     |
| [Kasichayanula 2011a](#5 References)                         | Fasted, single oral dose of 10 mg                            |
| [Kasichayanula 2011b](#5 References)                         | Control phases of study 1, 2 and 3<br />(single oral doses of 20 mg or 50 mg) |
| [Kasichayanula 2011c](#5 References)                         | Healthy subjects with a single oral dose of 10 mg            |
| [Kasichayanula 2012](#5 References)                          | Control phase with a single oral dose of 20 mg               |
| [Kasichayanula 2013a](#5 References)                         | Control phases of study 1 and 2<br />(single oral doses of 10 mg) |
| [Kasichayanula 2013b](#5 References)                         | Healthy subjects with normal kidney function<br />with a single oral dose of 50 mg |
| [Komoroski 2009](#5 References) and<br />[FDA Clinical Pharmacology Review for NDA 202293](#5 References) | SAD 2.5 to 500 mg (fasted)                                   |
| [Vakkalagadda 2016](#5 References)                           | Dapagliflozin only (single oral dose 10 mg)                  |

Kasichayanula *et al.* ([Kasichayanula 2008](#5 References)) investigated the mass balance of dapagliflozin in healthy subjects after a single oral dose of 50 mg. The following table gives an overview of the results:

| Output                     | reported | normalized** |
| -------------------------- | -------- | ------------ |
| Total recovery after 312 h | 96.15%   |              |
| Urine                      | 75.16%   |              |
| - unchanged                | 1.20%    | 1.23%        |
| - as metabolites           | 72.00%   | 73.93%       |
| Feces                      | 20.99%   |              |
| - unchanged                | 15.40%   | 18.90%       |
| - as metabolites           | 1.70%    | 2.09%        |

** to sum up to total excretion of urine and feces, respectively

The metabolic pattern was determined as shown in the following table.

| Output                              | reported | normalized** | add fraction excretion to feces of unchanged dapagliflozin to  glucuronides*** |
| ----------------------------------- | -------- | ------------ | ------------------------------------------------------------ |
| Dapagliflozin-3-O-glucuronide       | 60.70%   | 61.44%       | 78.80%                                                       |
| Dapagliflozin-2-O-glucuronide       | 5.40%    | 5.47%        | 7.01%                                                        |
| Dapagliflozin oxidative metabolites | 9.00%    | 9.11%        | 9.11%                                                        |
| **SUM**                             |          | **76.01%**   | **94.92%**                                                   |

** to sum to the values of metabolic quantifications from the table above (73.93% + 2.09%)

*** The fraction excretion to feces of unchanged dapagliflozin of 18.90% (see above) was added and distributed proportionally to Dapagliflozin-3-O-glucuronide and Dapagliflozin-2-O-glucuronide under the assumption that the measured fraction of unchanged dapagliflozin resulted from originally glucuronidated metabolites that underwent biliary excretion and subsequent degradation to dapagliflozin by bacterial glucurinodases in feces.

The following table shows the final mass balance data used for model building under the assumption of that unchanged dapagliflozin molecules in feces were originally glucuronides. Please refer to  [Section 2.3](#2.3 Model Parameters and Assumptions) for rationale.

| Observer                                                     | Value      |
| ------------------------------------------------------------ | ---------- |
| Fraction excreted  to urine of unchanged dapagliflozin       | 1.23%      |
| Fraction metabolized UGT1A9 (to  dapagliflozin-3-O-glucuronide) | 78.80%     |
| Fraction metabolized UGT2B7 (to  dapagliflozin-3-O-glucuronide) | 7.01%      |
| Fraction metabolized to oxidative  metabolites               | 9.11%      |
| **SUM**                                                      | **96.15%** |



#### 2.2.2.2	Model Verification

The following studies were used for model verification:

| Publication                                                  | Arm / Treatment / Information used for model verification    |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [Chang 2015](#5 References)                                  | Study 1 Treatment A (single oral dose of 5 mg as IC tablet) and<br /> Study 2 Treatment A (single oral dose of 10 mg as IC tablet) |
| [Komoroski 2009](#5 References) and<br />[FDA Clinical Pharmacology Review for NDA 202293](#5 References) | MAD 2.5 to 100 mg (day 1, 7 and 14)                          |
| [Komoroski 2009](#5 References)                              | Single oral dose 250 mg (fed)                                |


