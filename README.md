# Securing Configuration Settings in ASP.NET Core
Sample code for the blog post at https://mikaberglund.com/2019/09/09/store-your-app-service-configuration-settings-in-azure-key-vault/


## The Application

The application in this sample is a very simple ASP.NET Core application, which is based on the empty ASP.NET Core web application template in Visual Studio 2019, just to keep things as simple as possible.

When starting up, the application reads one configuration setting and writes that to the response, to show you how it works both locally, and in Azure when you deploy it. Naturally, this is not the way you should be writing your real-world applications.


## Configuration

Configuration files, such as `appsettings.Development.json`, are typically files that you exclude from source control in the [`.gitignore`](.gitignore) file. Usually, I create a markdown file that describes the contents and schema of the configuration file that has been excluded, to make it easier for new developers to get going.

Have a look at [`appsettings.Development.json.md`](AspNetCoreApp/appsettings.Development.json.md) for details.


## Live Demo

There is a live demo of this application available on Azure. [Have a look!](https://secure-settings-demo-web.azurewebsites.net/)