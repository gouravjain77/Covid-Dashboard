
# Covid 19 Reporting

## Project Description
In response to the global COVID-19 pandemic, this project was initiated to efficiently collect, process, and visualize data related to COVID-19 cases, deaths, hospital admissions, ICU occupancy, and testing statistics. Leveraging the capabilities of Azure Data Factory and Power BI, the project seamlessly integrates data retrieval, processing, storage, and dashboarding to provide actionable insights for stakeholders.

## Project Architecture
<img width="585" alt="Capture" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/da4d459e-2f62-4c4a-9305-c141a1ea8ebf">

## Key Steps in the Project:
### Data Retrieval and Storage
Data is fetched from the European Centre for Disease Prevention and Control (ECDC) website using an HTTP connector in Azure Data Factory.
The retrieved data is stored in a raw blob container within Azure Blob Storage, ensuring secure and scalable storage.
<img width="588" alt="data storage" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/803acec1-3c9c-4b8f-886a-363af3287e3b">

### Data Processing
Utilizing the dataflow feature in Azure Data Factory, the raw data undergoes comprehensive processing to transform it into a structured format suitable for analysis.

#### Cases and Deaths Data Transformation requirements -
<img width="705" alt="Transform_cases_deaths" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/737d0be2-f1b3-4513-a1f5-894744defd2c">

#### Dataflow Created for required Transformation -

<img width="759" alt="Transform_cases_deaths_dataflow" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/6ac87561-f0a7-46e3-b902-f8d9fda6f2a6">

#### Hospital Admissions Data Transformation requirements -

<img width="787" alt="transform_hospital_admissions" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/4a3da9cc-6113-4a98-988f-d3cb8784b9f9">

#### Dataflow Created for required Transformation -

<img width="817" alt="Transform_hospital_dataflow" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/254fc774-a17c-4932-a3d0-945dbc5f853a">


### Pipeline Creation
Three distinct pipelines - Cases and Deaths Data, Hospital Admissions Data, and Testing Data - are created within Azure Data Factory to orchestrate the data processing workflow efficiently.

#### Cases And Deaths Data Pipeline

<img width="445" alt="Final Pipeline Cases and deaths" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/7a1bc9a8-6b9d-4e56-a36e-4c62247072b6">

#### Hospital Admissions Data Pipeline

<img width="418" alt="Final Pipeline Hospital admissions" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/59b68b4e-f00a-40da-8905-189595cc2a90">

#### Testing Data Pipeline

<img width="283" alt="Final Pipeline Testing" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/0c5fe234-2536-441e-a7b2-0b48d09a3234">

### Automation and Monitoring
Scheduled triggers and failure alerts are implemented to automate the entire data processing system, ensuring timely updates and proactive identification of issues.

### Data Integration
Processed data is seamlessly copied to a SQL Server database, serving as a centralized source for Power BI visualization.

### Dashboard Development
Power BI is employed to develop a multipage dashboard encompassing COVID-19 metrics such as cases, deaths, hospital admissions, ICU occupancy, and testing data. The dashboard provides intuitive visualizations and interactive insights, empowering stakeholders to make informed decisions.

