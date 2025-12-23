# PROJECT1
**Patient Risk Assessment and Classification Module**

## 1. General Information

This project is a Python-based analytical module intended for patient risk assessment using physiological, biochemical, and clinical indicators.  
The module performs data normalization, categorical mapping, and qualitative risk classification.

The project is developed for educational and research purposes and can be used as a prototype of a decision-support system in healthcare analytics.

## 2. Purpose of the Project

The purpose of this project is to:
- process heterogeneous patient data (numerical and categorical);
- normalize indicators within predefined clinical bounds;
- convert qualitative symptom severity into quantitative values;
- classify an aggregated risk score into qualitative risk levels.

## 3. Scope of Application

The module can be applied in:
- medical and biomedical data analysis;
- educational projects in data science and applied analytics;
- research simulations using synthetic patient data;
- development of prototype clinical decision-support algorithms.

## 4. Technologies and Tools

The project uses the following technologies:

- **Programming language:** Python 3.x
- **Libraries:**
  - NumPy — numerical computations and array processing;
  - math — mathematical operations;
  - os — interaction with the operating system (reserved for future extensions).

No external databases or third-party frameworks are required.

## 5. Data Description

### 5.1 Input Parameters

Each patient profile may include the following indicators:

- blood glucose level;
- glucose trend;
- ketone concentration;
- insulin on board (IOB);
- time since last meal;
- symptom severity;
- heart rate and baseline heart rate;
- HbA1c level;
- time in range (TIR);
- coefficient of variation (CV);
- number of severe hypoglycemia episodes;
- albumin-to-creatinine ratio (ACR);
- LDL cholesterol level;
- duration of disease (years);
- number of comorbidities.

The dataset contains multiple synthetic patient cases representing different levels of risk, ranging from low to very high.

## 6. Functional Description

### 6.1 Data Normalization

Numerical indicators are normalized using a winsorized min–max approach, which limits extreme values within predefined bounds and reduces the impact of outliers.

### 6.2 Indicator Inversion

Certain normalized indicators may be inverted in cases where lower values correspond to higher clinical risk.

### 6.3 Symptom Severity Mapping

Qualitative symptom descriptions are mapped to numerical values to enable unified analytical processing.

### 6.4 Risk Categorization

The final risk score is classified into five qualitative categories:

- Very Low
- Low
- Medium
- High
- Very High

This classification provides an interpretable representation of patient risk.

## 7. Project Structure

The project has the following structure:

- main Python file containing helper functions and patient data;
- README file containing project documentation.

## 8. Limitations

- all patient data are synthetic and do not represent real clinical records;
- the module does not provide medical diagnoses;
- the results should not be used for clinical decision-making.

## 9. Possible Improvements

Potential future improvements include:
- implementation of a unified risk score calculation function;
- integration with real clinical datasets;
- visualization of patient risk profiles;
- exporting analytical results to external files or databases.

