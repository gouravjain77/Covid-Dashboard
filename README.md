
# Covid 19 Reporting

## Project Description
In response to the global COVID-19 pandemic, this project was initiated to efficiently collect, process, and visualize data related to COVID-19 cases, deaths, hospital admissions, ICU occupancy, and testing statistics. Leveraging the capabilities of Azure Data Factory and Power BI, the project seamlessly integrates data retrieval, processing, storage, and dashboarding to provide actionable insights for stakeholders.

## Project Architecture
<img width="585" alt="Capture" src="https://github.com/gouravjain77/Covid-Dashboard/assets/152005778/da4d459e-2f62-4c4a-9305-c141a1ea8ebf">

## Key Steps in the Project:
### Data Retrieval and Storage
Data is fetched from the European Centre for Disease Prevention and Control (ECDC) website using an HTTP connector in Azure Data Factory.
The retrieved data is stored in a raw blob container within Azure Blob Storage, ensuring secure and scalable storage.

### Data Processing
Utilizing the dataflow feature in Azure Data Factory, the raw data undergoes comprehensive processing to transform it into a structured format suitable for analysis.

### Pipeline Creation
Three distinct pipelines - Cases and Deaths Data, Hospital Admissions Data, and Testing Data - are created within Azure Data Factory to orchestrate the data processing workflow efficiently.

### Automation and Monitoring
Scheduled triggers and failure alerts are implemented to automate the entire data processing system, ensuring timely updates and proactive identification of issues.

### Data Integration
Processed data is seamlessly copied to a SQL Server database, serving as a centralized source for Power BI visualization.

### Dashboard Development
Power BI is employed to develop a multipage dashboard encompassing COVID-19 metrics such as cases, deaths, hospital admissions, ICU occupancy, and testing data. The dashboard provides intuitive visualizations and interactive insights, empowering stakeholders to make informed decisions.

