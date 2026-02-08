## Introduction

The National Health Interview Survey (NHIS) Adult Summary Health Statistics dataset, provided by the U.S. Centers for Disease Control and Prevention (CDC), contains aggregated survey data on health conditions, access to care, and unmet health needs for adults aged 18 and over. This dataset is broken down by condition, demographic group, and year, offering a rich resource to explore who gets help, who faces delays, and where invisible barriers exist in care-seeking. 

As a Datathon participant, your team is tasked with analyzing this data to uncover patterns, inequities, and insights about access to care. Your findings can help reveal barriers, suggest interventions, and tell a story about the human experience of navigating health systems.

This Datathon is your opportunity to dive deep into real-world health data, develop innovative analyses, and create data-driven insights that highlight friction, disparities, and opportunities for improvement in healthcare access.

## Tasks

Your task is to answer one or more of the following questions, or any question that sparks curiosity in you and your team regarding the dataset:

### Machine Learning Model

Teams interested in predictive modeling may attempt tasks such as:

- For a specific health topic and subgroup (e.g., angina in adults 65+), predict:
    - Estimated prevalence or percentage of delayed care for the next year
    - Projected unmet needs for that population
- For the dataset as a whole, predict trends in delayed or missed care over the next year
- Identify subgroups most at risk of falling through the cracks using clustering or anomaly detection techniques

### Data Analytics and Data Visualization

The following questions can be approached by both data analysts and visualization teams:

- Which subgroups experience the highest rates of delayed or unmet care?
- How do barriers differ by age, gender, income, or other demographic categories?
- Are there trends over time (2019–2023) in delayed care or health outcomes?
- How do patterns differ across health conditions or topics?
- Create visualizations showing where care breaks down or populations at risk
- Explore invisible barriers by comparing expected care availability to reported access

## Download the Dataset

Download the CSV here:

[NHIS Adult Summary Health Statistics](https://drive.google.com/file/d/1X2xzSyox19SJOxmtiYOijIa6TUqHi6wa/view?usp=sharing)

More info about the dataset: 

[CDC Data Page](https://data.cdc.gov/National-Center-for-Health-Statistics/DQS-NHIS-Adult-Summary-Health-Statistics/gj3i-hsbz/about_data)

### Dataset Columns

The dataset includes the following columns:

- `TOPIC`: Broad health topic or condition
- `SUBTOPIC`: More specific condition within the topic
    - Aggregate or pivot topics and subgroups for visualizations or clustering
- `GROUP` / `SUBGROUP`: Demographic breakdowns (e.g., age, gender)
- `TIME_PERIOD`: Year of data collection
- `ESTIMATE`: Numeric estimate (e.g., percentage of population affected)
- `STANDARD_ERROR`: Standard error of the estimate
- `ESTIMATE_LCI` / `ESTIMATE_UCI`: 95% confidence interval
- `FLAG` / `FOOTNOTE_ID_LIST`: Metadata or notes about data quality

**Recommended preprocessing:**

- Filter out rows with flags indicating unreliable estimates
- Consider creating derived metrics, such as differences between subgroups or year-over-year change
