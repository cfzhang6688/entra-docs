---
author: kengaderdus
ms.service: entra-external-id
ms.subservice: customers
ms.topic: include
ms.date: 03/08/2024
ms.author: kengaderdus
ms.manager: mwongerapk
---

To specify that this app is a public client and can use native authentication, enable public client and native authentication flows:
 
1. From the app registrations page, select the app registration for which you want to enable public client and native authentication flows.  
1. Under **Manage**, select **Authentication**.
1. Under **Advanced settings**, allow public client flows: 
    1. For **Enable the following mobile and desktop flows** select **Yes**.
    1. For **Enable native authentication**, select **Yes**.
1. Select **Save** button.

If you don't see the **Enable native authentication** option, add a *enableNativeAuthConfiguration=true* query parameter to your Microsoft Entra admin center URL, then load the page again with the new query parameter. For example, if the URL in your browser address bar is:

```http
https://entra.microsoft.com/view/Overview/appId/9b0eb21e-0c23-abc34t-98uhd
```

Update it to look similar to:

```http
https://entra.microsoft.com/?enableNativeAuthConfiguration=true#view/Overview/appId/9b0eb21e-0c23-abc34t-98uhd
```
Make sure you add the query parameter immediately after the domain.