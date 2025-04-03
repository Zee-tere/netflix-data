# Netflix Data Analysis

## Project Overview
This project involves the cleaning, wrangling, and analysis of a dataset containing Netflix original films, documentaries, and specials released as of June 1st, 2021. The dataset was web-scraped from Wikipedia and integrated with IMDb ratings. The goal of this analysis is to uncover insights into Netflix's content trends and performance using Python and Excel, ultimately preparing the data for visualization in Tableau.

## Dataset Context
The dataset consists of all Netflix original films along with metadata such as:
- **Title**: The name of the film
- **Genre**: The category of the film (e.g., Drama, Comedy, Documentary)
- **Original Premiere Date**: The date when the film was first released
- **Runtime**: Duration of the film in minutes
- **IMDB Score**: User ratings for the film as of June 1, 2021
- **Languages Available**: The languages in which the film can be streamed

## Data Cleaning and Wrangling
Several data preprocessing steps were applied to ensure the dataset's quality and usability. These steps include:

### 1. Handling Missing Values
- Checked for missing values and imputed or removed them based on context.
- Missing IMDb scores were either replaced with a placeholder or removed if critical to analysis.
- Missing genre values were filled using relevant external sources or marked as "Unknown."

### 2. Standardizing Columns
- Converted all text columns to a uniform case for consistency.
- Standardized date formats to `YYYY-MM-DD`.
- Ensured numerical columns (e.g., IMDb scores, runtime) had correct data types.

### 3. Introducing Additional Columns
- **Year of Release**: Extracted from the premiere date to analyze trends over time.
- **Month of Release**: Extracted to observe seasonal content release patterns.
- **Decade of Release**: Created to analyze content trends across different decades.
- **Content Type**: Classified titles as "Film," "Documentary," or "Special" based on genre.
- **IMDb Rating Category**: Grouped ratings into "Low" (0-4), "Average" (5-6.9), and "High" (7+).

### 4. Removing Duplicates
- Identified and removed duplicate entries to ensure accuracy.

### 5. Feature Engineering
- Extracted key insights by breaking down IMDb scores into categorical values for better visualization.
- Categorized film runtimes into short (<60 min), medium (60-120 min), and long (>120 min).

### 6. Data Formatting for Visualization
- Ensured data was structured appropriately for Tableau dashboarding.
- Exported the cleaned dataset in `.csv` and `.xlsx` formats for analysis.

## Next Steps
- Perform in-depth exploratory data analysis (EDA) to uncover trends.
- Create interactive visualizations in Tableau to highlight key insights.
- Compare Netflix's content strategy to competitors based on IMDb ratings and genre distribution.

## Tools Used
- **Python (Pandas, NumPy, Matplotlib, Seaborn)**: For data cleaning, manipulation, and initial visualization.
- **Excel**: For exploratory analysis and quick data validation.
- **Tableau**: For creating interactive and insightful visualizations.

## Conclusion
This project showcases advanced data wrangling techniques to prepare a real-world dataset for analysis. By leveraging structured cleaning and feature engineering, we enable meaningful insights into Netflix’s content trends and performance. The final analysis will provide a business-driven perspective on content strategy and viewer preferences.

---
For full access to the cleaned dataset and visualizations, visit the GitHub repository!

