# GL-Financial-Services
On a daily basis, multiple internal applications send large amounts of data (in CSV format) to the cloud storage location. Several data/schema validations need to be performed on this incoming data. Data will be persisted as a Delta table in Databricks once everything is passed.
# Tasks
--> Azure data lake storage is used by internal applications to store CSV files.

--> The following validation is needed to apply:

--> Make sure there are no duplicate rows. The file should be rejected if it contains duplicate rows.

--> Each date field needs to have its date format validated. Azure SQL server stores the name of the date column and the format in which it should be displayed. Failure to validate will result in the rejection of the file.

--> Put all rejected files in the Reject folder.

--> The passed files should be moved to the staging folder.

--> Create a Delta table in Azure Databricks with the passed files.
