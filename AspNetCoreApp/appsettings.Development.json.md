appsettings.Development.json
============================

The `appsettings.Development.json` configuration file should not be included in source control. In this sample application it is, just to make life easier for you.

To document configuration files that are required by the application, but excluded from source control, you can create a markdown file with the same name as the excluded file with the extension `.md` appended. In this file you can then document everything you want to document about the file, for instance:

## For Developers

If you don't have a `appsettings.Development.json` file in the same folder with this documentation, you need to create one. It is a standard ASP.NET Core configuration file, with the following additions used by the application.

``` JSON
{
    "mySecret": "{secret value}"
}
```

The values are described in more detail in the list below.

- `mySecret`: Just a sample configuration value that is stored in the configuration JSON file locally and in Key Vault when deploying to Azure.