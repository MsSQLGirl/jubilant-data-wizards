# Welcome to **From Oops to Ops: Incident Management with Notebooks**

Register / schedule: https://www.alldaydevops.com/2021-schedule
Tuesday October 28, 2021

Recording: **coming soon!**

Speaker:  
- Julie Koesmarno - http://mssqlgirl.com | http://linkedin.com/in/juliekoesmarno | [@MsSQLGirl](http://twitter.com/mssqlgirl)     

## Abstract
What if you can apply software engineering practices to your troubleshooting guides (TSGs) / knowledge base for your team’s on-call or for your customers? What if you can reduce stress and mistakes in your incident response workflow and activate a more scientific approach? 

Join this session to learn more about TSG Ops framework using Jupyter Notebook for executable and automatable troubleshooting guides / knowledge base. TSG Ops innovates incident response approach by applying software engineering practice in curating TSGs and activating our scientific approach when troubleshooting. We will share our learnings and our journey in implementing TSG Ops using open source technology, internally in Azure Data and externally for our Azure Data customers.

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
1. Incident Response – why is it hard (to scale)?
   More complex world == more automation, yet incident response are often considered as a last thing to do. Most engineers don't want to spend time on documenting, they want to spend time on coding. What if engineers code the troubleshooting guides, instead of writing static documentation?

2. Re-framing our approach to troubleshooting guides: software artefacts & Jupyter Notebooks
   Troubleshooting Guides are software artefacts. Jupyter Notebooks can be executed through command lines and can be parameterized therefore it's can be added as part of your automation. This includes testing automation as well as incident response automation. 

3. Implementation: Executable, reusable & automatable troubleshooting guides
   There are three automation categories: 
   1. Automate the Diagnostics / Root Cause Analysis (RCA).  
   2. Automate incident filing.  
   3. Automate mitigation steps.  

   A flow example of the Automate RCA: 
    - Use Power Automate or Azure Logic Apps to automate the flow, i.e. to automatically trigger when an email is received or if a new task is assigned to you, to send an email after a job is completed with diagnostic or mitigation results.   
    - Use Azure Automation account and jobs that gets called by Power Automate or Azure Logic Apps, to run a PowerShell script that invokes a notebook (either SQL or PowerShell kernel based).  
    - Use a Jupyter Notebook with SQL / PowerShell kernel that does a number of diagnostic queries (and mitigation if applicable).     

   Watch the demo video previously presented at Scottish Summit - Notebooks 101 for SQL People starting at minute [27:07](https://youtu.be/80L-UTOlknw?t=1627).
    - Use Azure Data Studio UI to convert one SQL script at a time.  
      Related blog post: https://www.mssqlgirl.com/inajiffy-converting-from-sql-scripts-to-notebook/
    - Use PowerShellNotebook module for bulk imports, specifically these cmdlets:    
        - `ConvertTo-PowerShellNotebook` to convert PowerShell scripts to Notebooks with PowerShell kernel.
        - `ConvertTo-SQLNotebook` to convert SQL scripts to Notebooks with SQL kernel.

## Examples of SQL related notebooks
1. Tiger Toolbox : 
    - SQL Assessment Toolkit: https://github.com/microsoft/sql-server-samples/tree/master/samples/manage/sql-assessment-api/notebooks 
    - SQL Hybrid Toolkit: https://github.com/microsoft/tigertoolbox/tree/master/SQL-Hybrid-Cloud-Toolkit/content 
2. Glenn Berry’s Diagnostic Notebooks for SQL Server and Azure SQL: https://glennsqlperformance.com/resources/ 
4. Rob Sewell’s Notebook: http://sqldbawithabeard.com https://github.com/SQLDBAWithABeard/JupyterNotebooks   
4. The SQL Diagnostic (Jupyter) Book by Emanuele Meazzo https://tsql.tech/the-sql-diagnostic-jupyter-book/ 

## Other useful resources
Submit your issues on Azure Data Studio: https://github.com/microsoft/azuredatastudio/issues 
