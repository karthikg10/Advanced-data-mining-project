# Data Analysis and User Behavior Profiling

This project consists of two Python scripts that leverage PySpark and data visualization libraries to analyze user activities and extract insights from datasets such as `logon_info`, `device_info`, and `http_info`. These scripts include detailed exploratory data analysis (EDA), feature engineering, clustering, and visualization.

---

## Scripts Overview

### 1. `data_analysis.py`

**Objective:** Perform detailed exploratory data analysis and generate visualizations for datasets including `logon_info`, `device_info`, and `file_info`.

#### Key Functionalities:
1. **Dataset Analysis:**
   - Loads datasets into PySpark DataFrames.
   - Identifies missing values and unique entries in critical columns.
   - Separates activities such as logon and logoff for individual analysis.

2. **Activity Trends:**
   - Analyzes trends in user activities, such as logon/logoff counts and device interactions, over time.
   - Extracts and visualizes the distribution of file types.

3. **User and Device Profiling:**
   - Identifies the top users and devices by activity count.
   - Clusters users based on their interaction patterns.

4. **Visualizations:**
   - Plots include:
     - Activity distribution over time.
     - Top users and devices by activity count.
     - File type distribution and upload trends.

#### Dependencies:
- PySpark
- Matplotlib
- Pandas
- WordCloud

#### How to Run:
1. Install dependencies:
   ```bash
   pip install pyspark matplotlib pandas
   ```
2. Run the script:
   ```bash
   python data_analysis.py
   ```
3. Ensure datasets (`logon_info.csv`, `device_info.csv`, `file_info.csv`) are in the specified paths.
   Feel free to reach out for the dataset accsess.
---

### 2. `adm_project.py`

**Objective:** Perform advanced profiling of user behavior and generate a unified report with key insights from multiple datasets.

#### Key Functionalities:
1. **Data Loading and Preprocessing:**
   - Loads datasets (`logon_info.csv`, `device_info.csv`, `http_info.csv`).
   - Converts date fields to a standard format and extracts relevant time-based features.

2. **User Behavior Analysis:**
   - Analyzes logon and logoff activities by hour.
   - Profiles device usage to identify frequently accessed PCs.
   - Determines top visited websites and frequent content keywords.

3. **Unified Reporting:**
   - Combines various analyses into a single PySpark DataFrame summarizing key findings (e.g., top sites, device usage, logon activities).

4. **Clustering:**
   - Groups users based on activities like logon, file access, and device interactions using KMeans.

5. **Visualizations:**
   - Includes plots for:
     - Hourly logon/logoff activity.
     - Most used devices.
     - Top visited websites.
     - Keyword frequencies.

#### Dependencies:
- PySpark
- Matplotlib
- Seaborn
- Pandas
- scikit-learn

#### How to Run:
1. Install dependencies:
   ```bash
   pip install pyspark matplotlib seaborn pandas scikit-learn
   ```
2. Run the script:
   ```bash
   python adm_project.py
   ```
3. Ensure datasets (`logon_info.csv`, `device_info.csv`, `http_info.csv`) are in the specified paths.

---

## Outputs
- **Unified Report:** Summarizes user behaviors across datasets.
- **Visualizations:** Graphs for activity trends, device usage, and keyword analysis.
- **Clustering Insights:** User groups with similar behaviors.

---

## Contribution
Contributions to enhance the functionality or improve visualizations are welcome. Submit a pull request with a clear description of your changes.

---

For further details or assistance, feel free to reach out!

