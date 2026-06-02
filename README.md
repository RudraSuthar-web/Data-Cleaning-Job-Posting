# Data Cleaning Job Posting

This project focuses on the cleaning and exploratory data analysis (EDA) of a job postings dataset to identify and analyze patterns, specifically targeting fraudulent job advertisements.

## Project Overview

The main objective is to preprocess the "Real or Fake: Fake Job Posting Prediction" dataset to make it suitable for further analysis or machine learning tasks. The project utilizes Python libraries such as Pandas for data manipulation and Plotly for interactive visualizations.

## Dataset

The dataset used is \`fake_job_postings.csv\`, located in the \`data/\` directory. It contains approximately 18,000 job postings with the following key features:

- **job_id**: Unique identifier for each job posting.
- **title**: The title of the job entry.
- **location**: Geographical location of the job.
- **department**: Corporate department (e.g., Sales, Engineering).
- **salary_range**: Indicative salary range.
- **company_profile**: A brief description of the company.
- **description**: Detailed description of the job.
- **requirements**: Pre-requisites for the job.
- **benefits**: Benefits offered by the company.
- **telecommuting**: Boolean flag for telecommuting positions.
- **has_company_logo**: Boolean flag indicating if a company logo is present.
- **has_questions**: Boolean flag indicating if screening questions are present.
- **employment_type**: Full-time, part-time, contract, etc.
- **required_experience**: Entry level, Associate, Mid-Senior level, etc.
- **required_education**: High School, Bachelor's Degree, etc.
- **industry**: The industry the company operates in.
- **function**: The job function (e.g., Marketing, IT).
- **fraudulent**: Target variable (0 for real, 1 for fake).

## Installation

To set up the environment, ensure you have Python installed and then install the required dependencies:

\`\`\`bash
pip install -r requirements.txt
\`\`\`

## Data Cleaning Workflow

The cleaning process performed in the \`Data_Cleaning_Job_Posting.ipynb\` notebook includes:

1.  **Handling Missing Values**:
    - Dropping columns with significant missing data: \`department\` and \`salary_range\`.
    - Removing rows where the \`description\` is missing.
    - Filling missing text values (\`company_profile\`, \`requirements\`, \`benefits\`) with "Not Provided".
    - Imputing missing categorical values (\`location\`, \`employment_type\`, etc.) with their respective modes.
2.  **Visualization**:
    - Analyzing the distribution of job locations and other categorical features using Plotly.

## Usage

You can explore the data cleaning steps and visualizations by running the Jupyter notebook:

\`\`\`bash
jupyter notebook notebook/Data_Cleaning_Job_Posting.ipynb
\`\`\`
