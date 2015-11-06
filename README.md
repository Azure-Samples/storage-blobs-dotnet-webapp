---
services: storage
platforms: dotnet
author: perrysk-msft
---

# storage-blobs-dotnet-webapp
Azure Blob Storage Photo Gallery Web Application using ASP.NET MVC 5. The sample uses the .NET 4.5 asynchronous programming model to demonstrate how to call the Storage Service using the Storage .NET client library's asynchronous APIs.
## Running this sample
1. Before you can run this sample, you must have the following perquisites:
	- An active Azure Storage account - If you don't have an account, refer to the [Create a Storage account](https://azure.microsoft.com/en-us/documentation/articles/storage-create-storage-account/) article.
	- Visual Studio 2015 (or higher).

2.Clone this repository using Git for Windows (http://www.git-scm.com/), or download the zip file.

3.From Visual Studio, open the **WebApp-Storage-DotNet.sln** file from the root directory.

4.In Visual Studio Build menu, select **Build Solution** (or Press F6).

5.Retrieve the STORAGE ACCOUNT NAME and PRIMARY ACCESS KEY (or SECONDARY ACCESS KEY) values from the Keys blade of your Storage account in the Azure Preview portal. For more information on obtaining keys for your Storage account refer to [View, copy, and regenerate storage access keys](https://azure.microsoft.com/en-us/documentation/articles/storage-create-storage-account/#view-copy-and-regenerate-storage-access-keys)

6.In the **Web.config** file, located in the project root, find the **StorageConnectionString** app setting and replace the placeholder values with the values obtained for your account.

  <add key="StorageConnectionString" value="DefaultEndpointsProtocol=https;AccountName=[Enter Your Storage AccountName];AccountKey=[Enter Your Storage AccountKey]" />

7.You can now run and debug the application locally by pressing **F5** in Visual Studio.

## Deploy this sample to Azure
1. In Visual Studio Solution Explorer, right-click on the project name and select **Publish...**

2. Using the Publish Website dialog, select **Microsoft Azure Web Apps**

3. In the next dialog, either select an existing web app, or follow the prompts to create a new web application. Note: If you choose to create a web application, the Web App Name chosen must be globally unique.

4. Once you have selected the web app, click **Publish**

5. After a short time, Visual Studio will complete the deployment and open a browser with your deployed application.

For additional ways to deploy this web application to Azure, please refer to the [Deploy a web app in Azure App Service](https://azure.microsoft.com/en-us/documentation/articles/web-sites-deploy/) article which includes information on using Azure Resource Manager (ARM) Templates, Git, MsBuild, PowerShell, Web Deploy, and many more.
## About the code
The code included in this sample is not intended to be a set of best practices on how to build scalable enterprise grade web applications. This is beyond the scope of this quick start sample.
## More information
- [What is a Storage Account](http://azure.microsoft.com/en-us/documentation/articles/storage-whatis-account/)
- [Getting Started with Blobs](http://azure.microsoft.com/en-us/documentation/articles/storage-dotnet-how-to-use-blobs/)
- [Blob Service Concepts](http://msdn.microsoft.com/en-us/library/dd179376.aspx)
- [Blob Service REST API](http://msdn.microsoft.com/en-us/library/dd135733.aspx)
- [Blob Service C# API](http://go.microsoft.com/fwlink/?LinkID=398944)
- [Delegating Access with Shared Access Signatures](http://azure.microsoft.com/en-us/documentation/articles/storage-dotnet-shared-access-signature-part-1/)
