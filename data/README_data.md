# Data Availability  
## Original Dataset  The original clinical dataset (58 patients with Takotsubo Syndrome, AOU Cagliari) cannot be shared publicly due to:  - Ethics Committee approval: AOU Cagliari, Protocol NP/2022/788 - Written informed consent limited to anonymised research use - Institutional data protection policies  Researchers wishing to access the original data may contact the corresponding author. 
## Synthetic Test Dataset  A synthetic dataset (`synthetic_test_dataset.csv`) is provided to verify that the code runs correctly. It replicates: - The same variable names and structure - Approximate marginal distributions (mean, SD) - Similar missing data patterns (proportions per variable)  This dataset does NOT contain real patient data and should NOT be used to draw clinical conclusions.  
## Using the Synthetic Dataset  Replace the data loading line in each notebook: ```python 
# Original (requires access to real data) df = pd.read_excel(DATA_PATH, engine='xlrd', sheet_name='Baseline')  
# Synthetic (for code verification) df = pd.read_csv('data/synthetic_test_dataset.csv') ```

