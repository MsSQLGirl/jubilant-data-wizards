# Welcome to Notebooks Deep Dive at Data Platform Summit 2021

## Useful References

1. 


### Launch and execute SQL Docs articles as notebooks in Azure Data Studio 

This is a preview feature for us to collect feedback from you. The docs articles that you can launch and execute as notebooks in Azure Data Studio are:
1. MSSQLSERVER_35250
https://docs.microsoft.com/sql/relational-databases/errors-events/mssqlserver-35250-database-engine-error
2. Troubleshoot a Full Transaction Log (SQL Server Error 9002)
https://docs.microsoft.com/sql/relational-databases/logs/troubleshoot-a-full-transaction-log-sql-server-error-9002


### Execute Notebook from CLI 
1. For PowerShell Notebooks: Use [Invoke-ExecuteNotebook](https://github.com/dfinke/PowerShellNotebook#executing-a-notebook)  
    This requires PowerShell 7.1.
2. For SQL Notebooks: Use [Invoke-SqlNotebook](https://docs.microsoft.com/powershell/module/sqlserver/invoke-sqlnotebook)
3. For Python Notebooks (including Kqlmagic): Use [Papermill](https://docs.microsoft.com/sql/azure-data-studio/notebooks/parameterize-papermill)


### Notebook Parameterization
When using Notebook Parameterization, you can use Python and PowerShell 7.1. You can create an "API" like to parameterize notebook execution. read more:
- [Create a parameterized notebook by using Papermill](https://docs.microsoft.com/sql/azure-data-studio/notebooks/parameterize-papermill)
- [Create a parameterized notebook by using the notebook URI](https://docs.microsoft.com/en-us/sql/azure-data-studio/notebooks/parameterize-uri)
- [Create a paramtereized notebook by using the Run with Parametes action](https://docs.microsoft.com/en-us/sql/azure-data-studio/notebooks/run-with-parameters)