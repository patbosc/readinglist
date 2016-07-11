#Azure
-----------------------------------------

##Service Bus

###Notifications Hub
- [Add Push Notifications to Asp.net MVC Web API](https://azure.microsoft.com/en-us/documentation/articles/notification-hubs-aspnet-backend-windows-dotnet-notify-users/)

##Azure Files
- [Azure Files](https://www.petri.com/configure-a-file-share-using-azure-files)

##Azure and VSTS you need this link
https://manage.windowsazure.com/publishsettings/index?client=vsserverexplorer&schemaversion=2.0

##Azure Webapp CI via MSBuild these parameters could be usefull when using asp.net mvc 4.x 
/p:WebPublishMethod=Package /p:PackageAsSingleFile=true /p:SkipInvalidConfigurations=true /p:PackageLocation="$(Build.StagingDirectory)" /p:DeployOnBuild=true
