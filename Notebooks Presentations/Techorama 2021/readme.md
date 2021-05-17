# Welcome to "From Oops to Ops: Incident Management with Notebooks"

Register / schedule: https://techorama.be/agenda?day=tuesday
Tuesday May 18, 2021 at 16:00 CET

## Abstract
What if you can apply software engineering practices to your troubleshooting guides (TSGs) / playbook / runbook for your team’s on-call? 
What if you can reduce stress and mistakes in your incident response workflow? 

Join this session to learn more about TSG Ops framework, where we revolutionize how Database Administrators and Data Engineers can be more effective
 and feel empowered during incident response. We will share some of our learnings and our journey on implementing TSG Ops, which is based on Jupyter Notebooks. 
 
 We’ll show how TSG Ops in Azure Data Studio makes incident response for SQL Server (on-prem) and Azure SQL much easier. We’ll show case how you can use 
 Notebooks with your favorite languages, from SQL to KQL, from PowerShell to Python, and all the way to .net interactive, providing you most flexibility.

 ## Useful references

 ### Pre-requisites:
 1. Azure Data Studio - download from [http://aka.ms/getAzureDataSTudio](http://aka.ms/getAzureDataStudio)
 2. Basic knowledge on Notebooks:
    - [Notebooks 101 for SQL people video tutorial](https://www.youtube.com/watch?v=80L-UTOlknw) from Scottish Summit channel, or
    - [Jupyter Notebooks for the mere mortals video tutorial](https://www.youtube.com/watch?v=-akGNOsaMg0) from Tech(K)now Day channel

### Topics covered:
1. Intro to TSG and Notebooks
2. Executable TSGs with Notebooks
3. Jumpstart your Notebooks
4. Automatable TSGs with Notebooks
    - Use Power Automate or Azure Logic Apps to automate the flow, i.e. to automatically trigger when an email is received or if a new task is assigned to you, to send an email after a job is completed with diagnostic or mitigation results. 
    - Use Azure Automation account and jobs that gets called by Power Automate or Azure Logic Apps, to run a PowerShell script that invokes a notebook (either SQL or PowerShell kernel based).
    - Use a Jupyter Notebook with SQL / PowerShell kernel that does a number of diagnostic queries (and mitigation if applicable).     
5. Takeaways and other resources
 