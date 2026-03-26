# Immigration Education Analysis

This project analyzes educational activity in Denmark based on data from Statistikbanken.

## Why this matters

Changes in student composition have direct implications for capacity planning, resource allocation, and targeted integration initiatives. Understanding these trends enables policymakers and institutions to anticipate shifts in demand and design more effective education and inclusion strategies.

## 📊 Dataset
The data comes from Statistics Denmark (DST) and includes:
- Educational activity in upper secondary education (gymnasiale uddannelser)
- Groups: 
  - Persons with Danish origin
  - Immigrants
  - Descendants
- Split by gender (men and women)
- Time period: 2015–2022

## 📁 Project Structure


ImmigrationEducation/
│
├── data/
│ ├── raw/ # Original CSV files
│ └── processed/ # Cleaned data
│
├── notebooks/
│ └── 01_data_overview.ipynb
│
├── outputs/ # Figures and results
├── src/ # Python scripts (future)
│
├── README.md
└── requirements.txt


## 🧹 Data Cleaning Steps

- Loaded raw CSV data from Statistikbanken
- Handled encoding issues (latin1)
- Selected relevant columns
- Renamed columns (years)
- Removed empty rows
- Added gender column
- Converted data from wide to long format using `pandas.melt()`

## 📈 Analysis

The dataset allows:
- Comparison between groups (Danish origin, immigrants, descendants)
- Comparison between genders
- Analysis of trends over time


## Results

### Men - all groups over time
![Men Plot](outputs/maend_grupper.png)
### Women - all groups over time
![Women Plot](outputs/kvinder_grupper.png)

### Immigrants - men vs women
![Immigrants Plot](outputs/indvandrere_kon.png)

## Insights
- The declining number of students with Danish origin suggests a structural shift in student composition.
- The increase in descendants until 2020 indicates a growing share of this group in upper secondary education.
- The decline in immigrant students until 2020, followed by a recovery, suggests sensitivity to external factors.
- Similar trends across genders indicate that changes are driven by broader demographic developments rather than gender-specific factors.
## Implications
- A declining number of students with Danish origin may require adjustments in capacity planning and resource allocation.
- The increasing share of descendants highlights a need for targeted support and integration initiatives.
- Fluctuations in immigrant student numbers suggest the importance of flexible planning and responsiveness to changing demand.
- The consistency across genders indicates that policy responses should focus on structural rather than gender-specific factors.

## Conclusion

This analysis shows a clear decline in students with Danish origin over time, while descendants have increased and immigrants show recovery after 2020.

The patterns are similar for men and women, suggesting that broader structural trends affect all groups.

Overall, the composition of students is gradually changing over time.

## ⚙️ Technologies

- Python
- Pandas
- Jupyter Notebook

## 🚀 How to run

1. Clone the repository
2. Install dependencies:

```bash
pip3 install -r requirements.txt
Open the notebook:
notebooks/01_data_overview.ipynb
📌 Author

Khalil Mashinesh
