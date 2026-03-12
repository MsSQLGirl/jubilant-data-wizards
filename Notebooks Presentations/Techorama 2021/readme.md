# Welcome to **From Oops to Ops: Incident Management with Notebooks**

Register / schedule: https://techorama.be/agenda?day=tuesday.  
Tuesday May 18, 2021 at 16:00 CET.  

Speakers:  
- Julie Koesmarno - http://mssqlgirl.com | http://linkedin.com/in/juliekoesmarno | [@MsSQLGirl](http://twitter.com/mssqlgirl)     
- Shafiq Rahman - https://www.linkedin.com/in/shafiq-rahman-16853a5/  

## Abstract
What if you can apply software engineering practices to your troubleshooting guides (TSGs) / playbook / runbook for your team’s on-call? 
What if you can reduce stress and mistakes in your incident response workflow? 

Join this session to learn more about TSG Ops framework, where we revolutionize how Database Administrators and Data Engineers can be more effective
and feel empowered during incident response. We will share some of our learnings and our journey on implementing TSG Ops, which is based on Jupyter Notebooks. 
 
We’ll show how TSG Ops in Azure Data Studio makes incident response for SQL Server (on-prem) and Azure SQL much easier. We’ll show case how you can use 
Notebooks with your favorite languages, from SQL to KQL, from PowerShell to Python, and all the way to .net interactive, providing you most flexibility.

## Useful pre-reads:
1. Azure Data Studio.  
    - Download from http://aka.ms/getAzureDataStudio.  
2. Basic knowledge on Notebooks:  
    - [Notebooks 101 for SQL people video tutorial](https://www.youtube.com/watch?v=80L-UTOlknw) from Scottish Summit channel, or  
    - [Jupyter Notebooks for the mere mortals video tutorial](https://www.youtube.com/watch?v=-akGNOsaMg0) from Tech(K)now Day channel.  
3. PowerShellNotebook module.
    - [Invoke-PowerShellNotebook](https://github.com/dfinke/PowerShellNotebook).  
    - Related video: https://www.youtube.com/watch?v=3b_LQn18oHI.  
4. SqlServer module.
    - [Invoke-SqlNotebook](https://docs.microsoft.com/powershell/module/sqlserver/invoke-sqlnotebook)

## Topics covered:
1. Intro to TSG and Notebooks.  
   Our studies in Incident Response scenarios show that DBAs / Data Professionals still use static documents (Word, OneNote, Wiki) as Knowledge Base or troubleshooting guides. While traditionally this is OK, as data estate and ecosystems become more complex, we think that treating troubleshooting guides as code will help with maintainability and scalability. Azure Data Studio is continuously pushing for improvements in Notebooks that are ideal for supportability stories. 
2. Executable TSGs with Notebooks.  
    - Parameterization with Papermill.  
      See examples: [Parameterizing notebooks to investigate Azure SQL's log stored in Azure Log Analytics](https://github.com/MsSQLGirl/jubilant-data-wizards/blob/main/Simple%20Demo/Parameterization/SQLDBLog/Demo-ExecuteAzureSQLLogAnalytics.ipynb)  
      Related blog post: https://www.mssqlgirl.com/executing-a-parameterized-notebook-in-azure-data-studio/.  
    - Official documentation: [Create a parameterized notebook](https://docs.microsoft.com/sql/azure-data-studio/notebooks/notebooks-parameterization).  
3. Jumpstart your Notebooks.  
   Watch the demo video previously presented at Scottish Summit - Notebooks 101 for SQL People starting at minute [27:07](https://youtu.be/80L-UTOlknw?t=1627).
    - Use Azure Data Studio UI to convert one SQL script at a time.  
      Related blog post: https://www.mssqlgirl.com/inajiffy-converting-from-sql-scripts-to-notebook/
    - Use PowerShellNotebook module for bulk imports, specifically these cmdlets:    
        - `ConvertTo-PowerShellNotebook` to convert PowerShell scripts to Notebooks with PowerShell kernel.
        - `ConvertTo-SQLNotebook` to convert SQL scripts to Notebooks with SQL kernel.
4. Automatable TSGs with Notebooks.  
   There are three automation categories: 
   1. Automate the Diagnostics / Root Cause Analysis (RCA).  
   2. Automate incident filing.  
   3. Automate mitigation steps.  

   A flow example of the Automate RCA: 
    - Use Power Automate or Azure Logic Apps to automate the flow, i.e. to automatically trigger when an email is received or if a new task is assigned to you, to send an email after a job is completed with diagnostic or mitigation results.   
    - Use Azure Automation account and jobs that gets called by Power Automate or Azure Logic Apps, to run a PowerShell script that invokes a notebook (either SQL or PowerShell kernel based).  
    - Use a Jupyter Notebook with SQL / PowerShell kernel that does a number of diagnostic queries (and mitigation if applicable).     
5. Takeaways and other resources  


## Examples of SQL related notebooks
1. Tiger Toolbox : 
    - SQL Assessment Toolkit: https://github.com/microsoft/sql-server-samples/tree/master/samples/manage/sql-assessment-api/notebooks 
    - SQL Hybrid Toolkit: https://github.com/microsoft/tigertoolbox/tree/master/SQL-Hybrid-Cloud-Toolkit/content 
2. Glenn Berry’s Diagnostic Notebooks for SQL Server and Azure SQL: https://glennsqlperformance.com/resources/ 
4. Rob Sewell’s Notebook: http://sqldbawithabeard.com https://github.com/SQLDBAWithABeard/JupyterNotebooks   
4. The SQL Diagnostic (Jupyter) Book by Emanuele Meazzo https://tsql.tech/the-sql-diagnostic-jupyter-book/ 

## Other useful resources
Submit your issues on Azure Data Studio: https://github.com/microsoft/azuredatastudio/issues 
