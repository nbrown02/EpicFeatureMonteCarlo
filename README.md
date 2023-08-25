# Epic & Feature Monte Carlo

### What is this report? 
This will detail, based on your historical Throughput (completed backlog items/user stories), the likely completion date of Epics (if using Jira) or Features (if using Azure DevOps) based on the number of child items and a forecasted target date, as well as accounting for Epic/Feature work in progress.

### Why would you use it? 
Forward planning for a given period (e.g. a quarter) and projecting the likely completion of work. Managing expectations around delivery and better understanding of the impact the amount of things you are working on at any given time (WIP) has on your Feature delivery.

### When would you use it?
Use this when trying to understand what Epics/Features you are likely to deliver and when they will be delivered, ideally viewing this on a regular (weekly) basis

### Prerequisites
* [Make sure you have the latest version of Power BI Desktop](https://aka.ms/pbiSingleInstaller)
* Download the appropriate template file:
  - [Jira version](https://github.com/nbrown02/Flow-Metrics-Epics-Features/raw/main/Flow%20Metrics%20for%20Epics%20and%20Features%20(Jira).pbit)
  - [Azure DevOps version](https://github.com/nbrown02/Flow-Metrics-Epics-Features/raw/main/Flow%20Metrics%20for%20Epics%20and%20Features%20(Azure%20DevOps).pbit)
* If you are setting this up for Jira then [follow these steps](https://support.atlassian.com/atlassian-account/docs/manage-api-tokens-for-your-atlassian-account/) to setup a Jira API token and note it down (e.g. copy/paste into Notepad)
* If you are setting this up for Azure DevOps then [follow these steps](https://learn.microsoft.com/en-us/azure/devops/organizations/accounts/use-personal-access-tokens-to-authenticate?view=azure-devops&tabs=Windows#create-a-pat) to setup a Personal Access Token (PAT) with full access and note it down (e.g. copy/paste into Notepad)
* Then you're good to get started!

### Connectivity & Data Load
* Open the relevant .pbit file in Power BI Desktop
* For Jira:
  - Add your Jira URL
  - Add your Jira Project Key(s)
* For Azure DevOps:
  - Select http/https (only choose http if your Azure DevOps Server is HTTP)
  - Add the Analytics / Azure DevOps Server URL - for Azure DevOps services enter 'analytics.dev.azure.com' / for Azure DevOps Server enter your server details
  - Add your organization / project name / team name

* It should then look something like this (for Jira):
![alt text](https://raw.githubusercontent.com/nbrown02/Flow-Metrics-Epics-Features/main/Screenshots/1%20-%20Jira.jpg)

* Or this (for Azure DevOps):
![alt text](https://raw.githubusercontent.com/nbrown02/Flow-Metrics-Epics-Features/main/Screenshots/1%20-%20ADO.jpg)

* Hit 'Load' 
* You will be prompted for a login
* For Jira, choose Basic and enter:
  - Your email associated with your Jira account for your username
  - Your API token you created in the Prerequisities

![alt text](https://raw.githubusercontent.com/nbrown02/FlowViz-Jira/main/Screenshots/Login2.png)

* For Azure DevOps, choose Basic and enter:
  - Your Personal Access Token (PAT) to login, entering it in the password field (user can be left as blank - make sure it has 'Read' access to Analytics)

![alt text](https://docs.microsoft.com/en-us/azure/devops/report/powerbi/media/authentication-7.png?view=azure-devops)

* Then hit 'Connect' and wait for the data and charts to load!

### Screenshots

![alt text](https://raw.githubusercontent.com/nbrown02/EpicFeatureMonteCarlo/main/FMC4.gif)


### Feedback
This template is built and maintained by [Nicolas Brown](https://www.nicolasbrown.co.uk/) use [the issues section]((https://github.com/nbrown02/EpicFeatureMonteCarlo/issues)) for any bugs you find and [the discussion section](https://github.com/nbrown02/Flow-Metrics-Epics-Features/discussions) for any question, ideas and/or feature requests.
