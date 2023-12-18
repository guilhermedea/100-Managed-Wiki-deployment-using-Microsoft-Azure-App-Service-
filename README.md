# 100% Managed Wiki deployment using Microsoft Azure App Service (Docker-based) and Azure Database for PostgreSQL Servers

![picture with the words Cloud Project and icons of the services used](https://miro.medium.com/v2/resize:fit:720/format:webp/0*FeoQJYJ7RHEu2Xz_.jpg)

In this project based on a real-world scenario, I worked as a Cloud Engineer to deploy a Wiki to the cloud, 100% web, with access
for all team members. This enabled collaborative document creation, and all team members could see the latest version of the
document and propose improvements, allowing the team to better organize and manage documents.

To this solution deployment, I used Azure Database for PostgreSQL Servers and Azure App Service.

All important, procedural and operational documents, such as Runbooks and Knowledge Bases (KBs), which must always be available and
are constantly updated, were no longer stored locally (standalone), avoiding data inconsistencies.

![picture showing a graph of the solution architecture](https://miro.medium.com/v2/resize:fit:720/format:webp/0*2vVsGjSQVA05RFlS.jpg)

This project was made possible thanks to containerization technology, which combined with dynamic and integrated provisioning of Azure, 
allowed for quick and always available deployment. First, I created a PostgreSQL database in Azure itself, allowing internal connection 
between Azure services. Then I created a web app in Azure App Service, configuring it as a container. In this process, I also pointed to 
the Requarks Wiki image, an open-source software for creating Wikis, which was hosted on Docker Hub.

![picture of the installation screen of Wiki.js on a browser window](https://miro.medium.com/v2/resize:fit:720/format:webp/0*8T2veSTI7rQ2IgBc.png)

To finish the Azure App Service settings I just had to enter some values related to the database through the console interface and restart the container.
After that I logged on the container through the URL and finished installing Requarks Wiki. That’s it! The wiki system was already online, ready to be 
operated and 100% available on the web! Requarks Wiki brings powerful integrations, especially with cloud providers: it is possible to use AzureAD for
logins and Azure Blob Storage Service for performing periodic backups, for example.

This project was executed very quickly and practically, thanks to containerization technology, which combined with Azure’s dynamism, allows tasks that
would previously take hours of work to be executed in minutes, quickly, accessibly and persistently.


