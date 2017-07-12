Office Developer Resources
----------------------------

Connect
------
In this section you will find Links that are Helpfull for integrating Office APIs into you own projects.

Graph Explorer
------
- [Overview Microsoft Graph](http://graph.microsoft.io/en-us/)
- [Microsoft Graph Explorer](https://graph.microsoft.io/en-us/graph-explorer)
- [Office 365 API Reference Documentation](https://msdn.microsoft.com/office/office365/api/api-catalog)
- [Office 365 API Sandbox](https://apisandbox.msdn.microsoft.com/)
- [Active Directory Explorer check for /Applications](https://graphexplorer.cloudapp.net/)
> Note: API Call looks like this 'https://graph.windows.net/EasySchriftwechselNext.onmicrosoft.com/applications'
- [Well Known Url](https://login.windows.net/EasySchriftwechselNext.onmicrosoft.com/.well-known/openid-configuration)

ADAL
------ 
- [Azure AD Overview](https://msdn.microsoft.com/en-us/library/azure/dn645542.aspx)
> Note: Here is how you [add a Directory to your Azure Account](http://www.clemensreijnen.nl/post/2014/07/11/Add-an-existing-Office-365-Azure-Active-Directory-to-your-Azure-Subscription). Very Very Usefull to do [this](https://azure.microsoft.com/en-us/documentation/articles/active-directory-how-subscriptions-associated-directory/).
- [Here is how to setup the app in Azure AD](https://github.com/OfficeDev/TrainingContent/blob/master/O3653/O3653-1%20Deep%20Dive%20into%20Azure%20AD%20with%20the%20Office%20365%20APIs/Lab.md)
- [Azure AD Integration](https://msdn.microsoft.com/en-us/library/mt622431.aspx)
- [Curl Authentication Flow for Dynamics CRM](https://blogs.msdn.microsoft.com/crm/2013/12/12/use-oauth-to-authenticate-with-the-crm-service/)
- [ADAL SDK Platforms](https://azure.microsoft.com/en-us/documentation/articles/active-directory-authentication-libraries/)
- [ADAL.js](https://github.com/AzureAD/azure-activedirectory-library-for-js)
- [ADAL .net Nuget](https://www.nuget.org/packages/Microsoft.IdentityModel.Clients.ActiveDirectory)
- [ADAL .net Github](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet)
- [ADAL .net Documentation](https://msdn.microsoft.com/library/azure/mt417579.aspx)
> Note: OAuth Flow in Action see Outlook OAuth Flow
- [OAuth Notes from Meeting with Partner as PDF](oauthopenconnect.pdf)

Onedrive
---
- [Upload File REST API Call](http://graph.microsoft.io/docs/api-reference/v1.0/api/item_uploadcontent)

Extend
---
Here you can find everything around extending Office.

- [Overview](http://dev.office.com/docs/add-ins/overview/office-add-ins)
- [Availability](http://dev.office.com/add-in-availability)
- [Understanding Office.js](http://dev.office.com/docs/add-ins/develop/understanding-the-javascript-api-for-office)
- [Office.js Reference Documentation](http://dev.office.com/reference/add-ins/javascript-api-for-office)
- [Add-Ins Changelog](http://dev.office.com/changelog)
- [Wikipedia App Source Code](https://github.com/OfficeDev/Office-Apps)
- [Training Content](https://github.com/OfficeDev/TrainingContent/tree/master/O3652)


Outlook
---

Since Outlook is a System of it's own here are some usefull outlook things.

- [dev.outlook.com Code Samples](https://dev.outlook.com/Samples)
- [Authentication in Outlook](https://dev.office.com/docs/add-ins/outlook/authentication)
- [OAuth Flow MSDN Blogpost](https://blogs.msdn.microsoft.com/exchangedev/2014/10/28/oauth2-in-action-with-the-release-of-office-365-calendar-contacts-and-mail/)
- [OAuth Playground](https://oauthplay.azurewebsites.net/)

Manifest
---
- [Manifest Specify Host](https://dev.office.com/docs/add-ins/overview/specify-office-hosts-and-api-requirements)
- [Manifest Example for Command Add-in Outlook](https://github.com/jasonjoh/command-demo/blob/master/command-demo-manifest.xml)
- [Manifest Command-Sample (Ribbion Integration)](https://github.com/OfficeDev/Office-Add-in-Commands-Samples)

> Note: that the Manifest does not support &amp 

Random
---
[Blog Post from Richard about Office Identity Crisis - Extremly helpfull with Outlook Add-Ins](http://blogs.msdn.com/b/richard_dizeregas_blog/archive/2015/08/10/connecting-to-office-365-from-an-office-add-in.aspx)

Skype SDK's
---
[Overview Skype for Business SDK's](https://msdn.microsoft.com/en-us/library/mt124990.aspx)

Submission to the Store
---
- [Naming best Practices / Micorosft Office Store what Titels Names are allowed?](https://msdn.microsoft.com/en-us/library/office/jj635874.aspx)
- [Best Practices](https://dev.office.com/docs/add-ins/design/add-indevelopment-best-practice)
- [Policy Guidance](https://dev.office.com/blogs/Office-Store-Policy-andGuidance-Updates)

- [Starbucks - Best Practices](https://store.office.com/en-001/app.aspx?assetid=WA104380233&sourcecorrid=7cda4969-4691-44a1-9bc2-0424663dd855&searchapppos=0&ui=en-US&rs=en-001&ad=US&appredirect=false)
- [FindTime - Best Practices](https://store.office.com/en-001/app.aspx?assetid=WA104379803&sourcecorrid=af8847e8-d3ad-48c3-99cf-2b6649e0e7fa&searchapppos=0&ui=en-US&rs=en-001&ad=US&appredirect=false)

http://dev.office.com/docs/add-ins/outlook/troubleshoot-outlook-add-in-activation

Office Store
---

Pricing
-- 
[Some ISVs ask a lot about how to earn money with office add-ins ... details ...](https://dev.office.com/officestore/docs/decide-on-a-pricing-model)

Best Practices
--
Starbucks
https://store.office.com/en-us/app.aspx?assetid=WA104380233&sourcecorrid=f88a9bf4-fe31-4140-b9c3-86792507933d&searchapppos=0&ui=en-US&rs=en-US&ad=US&appredirect=false
Findtime
https://store.office.com/en-us/app.aspx?assetid=WA104379803&sourcecorrid=4d74136c-afc7-482c-915c-9049958af42d&searchapppos=0&ui=en-US&rs=en-US&ad=US&appredirect=false

Privacy and Security
--
[dev.office.com](https://dev.office.com/docs/add-ins/develop/privacy-and-security)

Here are the guidelines:
--
https://dev.office.com/officestore/docs/validation-policies
Seller Dashboard:
https://dev.office.com/officestore/docs/use-the-seller-dashboard-to-submit-to-the-office-store

http://sellerdashboard.microsoft.com

Manifest must Provide Support Link
Manifest for Outlook or Exchange must Provide Ribbon Integration

Conventions for Brand and Naming:
--
https://dev.office.com/officestore/docs/create-effective-office-store-listings
Validation Policy
https://dev.office.com/officestore/docs/validation-policies
