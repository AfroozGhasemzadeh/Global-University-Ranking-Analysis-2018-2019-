# Global-University-Ranking-Analysis-2018-2019-
Data cleaning and visualization project analyzing the 2018–2019 Global University Ranking dataset. Includes full preprocessing of corrupted and inconsistent data, feature engineering, geographic mapping, and ranking‑feature analysis. 
# 📌 Project Overview
This project analyzes the 2018–2019 University World Ranking dataset, focusing on transforming a messy real‑world dataset into a clean, structured, and insightful analysis. The dataset includes global university rankings and several academic performance indicators such as research output, faculty quality, alumni employment, and citation influence.
The raw data contains numerous inconsistencies — including corrupted text, missing values, non‑numeric ranking fields, and formatting issues — making it an excellent example of practical data‑cleaning and exploratory‑analysis skills.
This repository demonstrates a complete workflow:
* Cleaning and standardizing the dataset
* Converting ranking features into numeric form
* Correcting corrupted university names
* Exploring global and country‑level ranking patterns
* Visualizing geographic distribution and feature relationships
* Saving all figures into a dedicated folder for reproducibilit
# 📂 Dataset Source
The dataset originates from Kaggle:
University World Ranking (2018–2019)
/kaggle/input/university-world-ranking/eighteen_nineteen_university_datasets.csv
In this repository, the dataset is stored locally in:
dataset/eighteen_nineteen_university_datasets.csv
The notebook loads it using:
data = pd.read_csv(r"dataset\eighteen_nineteen_university_datasets.csv", encoding='unicode_escape')
# 📊 Dataset Features
The dataset includes the following columns:
* World Rank
* Institution
* Location
* National Rank
* Quality of Education
* Alumni Employment
* Quality of Faculty
* Research Output
* Quality Publications
* Influence
* Citations
* Score
These features form the basis of the ranking system and are used throughout the analysis.
# 🧹 Data Cleaning Summary
The raw dataset required extensive cleaning due to multiple issues:
1. Numerical features stored as strings
Many ranking‑related columns contained:
*  "-"
*  " " (extra spaces)
*  "?"
*  ">1000"
All were converted to numeric format.
Values like ">1000" were replaced with 1001 to preserve ranking order.
2. Corrupted university names
Some institution names contained:
 *  ?  characters
*  broken Unicode
*  unreadable text
These were cleaned and standardized into a new column: Institution_cleaned
3. Missing values
Missing entries were replaced or imputed depending on the feature.
# 🌍 Visualizations
All generated figures are saved automatically in the Figures/ folder.
The project includes:
* Global map showing where top universities are concentrated
* Countplot of universities per country
* Feature comparison plots for USA universities
* Scatter plots showing feature relationships
* Distribution plots for ranking features
# 🛠️ Libraries Used
This project uses the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- kaleido (for saving Plotly figures)
# 🚀 How to Run the Project
This project is implemented as a Jupyter Notebook.
1. Clone the repository
2. Install required libraries
3. Ensure the dataset is in the correct folder
4. Open the notebook
5. Run all cells
# 📝 Conclusion
This project demonstrates:
- Strong data‑cleaning and preprocessing skills
- Ability to handle corrupted and inconsistent real‑world data
- Clear visualization and analytical storytelling
- Understanding of ranking metrics and feature relationships
- Professional project organization suitable for portfolio and job applications
It serves as a strong example of practical data‑analysis skills for academic, research, or industry roles.

 


