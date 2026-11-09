[README (1).md](https://github.com/user-attachments/files/34575284/README.1.md)
# AI Usage and Impact on Students and Professionals

An end-to-end data analysis project that evaluates how generative AI adoption affects learning efficiency, productivity, and critical thinking habits across academic and professional groups. I cleaned, transformed, and visualized survey and behavioral data to uncover key usage trends.

## Tools Used

- PostgreSQL (pgAdmin 4): storing the raw data and cleaning it with SQL
- Excel: exporting and reviewing the cleaned dataset
- Power BI: building an interactive two-page dashboard

## Dataset

- 300 raw survey records, 288 after cleaning
- Fields include: user ID, age, gender, country, user type (student or professional), education level, profession, AI tool used, AI purpose, daily AI usage hours, hours saved per week, productivity score, satisfaction score, monthly income, and monthly AI cost

## Project Workflow

### 1. Raw data
The data was loaded into a raw PostgreSQL table (`aiusage_raw`). It had inconsistent text casing, missing values, and invalid entries such as ages written as "16 yrs".

### 2. Data cleaning (SQL)
- Standardized text casing for gender, country, and education level
- Converted ages with text, such as "23 yrs", into numbers
- Replaced blank categorical values with "Unknown"
- Created a clean table (`aiusage_clean`) with proper data types and a primary key on `UserID`

### 3. Dashboard (Power BI)
The cleaned data was modeled in Power BI across two report pages.

Page 1: adoption and purpose
- How evenly is user adoption distributed across the available AI tools?
- Which AI tools are most commonly used for each specific purpose?

Page 2: productivity and time saved
- What is the overall average productivity score across all users?
- What is the total estimated number of hours saved per week by AI adoption?
- Which AI tools yield the highest average time saved per week?
- How does daily AI usage vary across different professions?

## Key Findings

- ChatGPT dominates adoption, with about 42% of users, followed by Google Gemini at roughly 13%.
- 12 AI tools appear in the dataset.
- ChatGPT leads for coding and writing, the two most common purposes.
- The average productivity score is 4.98.
- AI adoption saves an estimated 1,620 hours per week across all users.
- Daily AI usage varies widely by profession, with research and AI-related roles using AI the most.

## Repository Contents
[Uploading aiusage.sql…]()

| File | Description |
|------|-------------|
| `aiusage.xlsx` | Cleaned dataset |
| `aiusage.sql` | SQL scripts used to clean the data |
| `powerbi1.pbix` | Power BI dashboard file |
| `screenshots/` | Raw data, clean data, and dashboard screenshots |

## Author

**Joseph Etim**, Database Analyst | Data Analysis & Query Development | SQL Expert

- Email: joeetim2001@gmail.com
- LinkedIn: [joseph-etim-69a408331](https://www.linkedin.com/in/joseph-etim-69a408331)
