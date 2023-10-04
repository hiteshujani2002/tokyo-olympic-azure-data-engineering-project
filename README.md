
# Tokyo Olympic Data Engineering Project

The Project Tokyo Olympic on Azure is a data processing project that utilizes Azure services to manage and transform Olympic dataset sourced from Kaggle. This README provides an overview of the project and its setup to help you get started.




## Project Image
![Data_Engineering_Project_Design drawio](https://github.com/hiteshujani2002/tokyo-olympic-azure-data-engineering-project/assets/84509735/e3d62501-2812-4a11-8a5f-b89173b35b1f)
## Project Workflow

- ### Azure Storage Account Creation: 
 We start by creating an Azure Storage Account. Within this account, we enable the hierarchical namespace feature to store data in a structured, hierarchical format.

- ### Data Organization: 
We create two folders within the storage account: raw-data and transformed-data. The raw-data folder is where we store the original, unprocessed data, while the transformed-data folder houses the data after it has undergone transformation using Azure Databricks.

- ### Data Ingestion with Data Factory: 
We create an Azure Data Factory pipeline to ingest data from various sources, including athletes.csv, entriesgender.csv, medals.csv, coaches.csv, and teams.csv, into the raw-data folder in Azure Data Lake Storage. This step ensures that the data is readily available for processing.

- ### Azure Databricks Transformation: 
We launch an Azure Databricks workspace and write transformation code to process the data. The transformed data is then loaded back into the Azure Data Lake Storage, specifically into the transformed-data folder. This step completes the data processing cycle.

- ### Data Analysis with Azure Synapse Analytics: 
We connect the Azure Data Lake Storage with Azure Synapse Analytics to perform data analysis. SQL scripts can be run on the data to gain valuable insights.












## Setup

- To set up and run the project locally or on your Azure account, follow these steps:

- Azure Account: Ensure you have an active Azure account. If not, sign up for one here.

- Kaggle Dataset: Obtain the Olympic dataset from Kaggle and save it to a local directory or a GitHub repository.

- Azure Storage Account: Create an Azure Storage Account through the Azure Portal.

- Azure Data Lake Storage: Within the storage account, configure Azure Data Lake Storage Gen2 and enable the hierarchical namespace.

- Data Factory Pipeline: Set up an Azure Data Factory pipeline to ingest data from Kaggle or your chosen source into the raw-data folder in Azure Data Lake Storage.

- Azure Databricks Workspace: Create an Azure Databricks workspace and set up notebooks to process and transform the data.

- Data Analysis with Azure Synapse Analytics: Connect Azure Synapse Analytics to the Azure Data Lake Storage and create SQL scripts for data analysis.

## Project Screenshots

- Creating data pipeline to ingest data from githu to Azure Data Lakes Gen2 storage

![Screenshot (3133)](https://github.com/hiteshujani2002/tokyo-olympic-azure-data-engineering-project/assets/84509735/fd9825e0-b7e5-412f-9b9a-91d43756da17)


- Synapse Workspace to perform analytics

![Screenshot (3135)](https://github.com/hiteshujani2002/tokyo-olympic-azure-data-engineering-project/assets/84509735/5c26859a-909a-49ff-b4e6-84d9863b2436)





## Tech Stack

- **Data Ingestion**: Data Factory
- **Data Storage**: Azure Data LakesGen2
- **Data Transformation**:Azure DataBricks 
- **Data Analytics**:Synapse Analytics


![Microsoft-Azure-Logo-2017](https://github.com/hiteshujani2002/tokyo-olympic-azure-data-engineering-project/assets/84509735/d4dd01f7-7e10-48f5-ba78-1cedd6a940b5)

