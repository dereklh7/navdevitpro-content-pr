---
title: Get userPermission | Microsoft Docs
description: Gets userPermission objects in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: henrikwh, SusanneWindfeldPedersen

ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/19/2018
ms.author: henrikwh, solsen
---

# Get userGroupMembers
Retrieve the properties and relationships of an userGroupMembers object for [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)].

## HTTP request
```
GET /microsoft/automation/{apiVersion}/companies({companyId})/users({userSecurityID})/userPermissions
```

## Request headers
|Header|Value|
|------|-----|
|Authorization  |Bearer {token}. Required. |

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a ```200 OK``` response code and list of  **userPermission** objects in the response body.

## Example

**Request**

Here is an example of the request.
```json
GET https://api.businesscentral.dynamics.com/v1.0/api/microsoft/automation/beta/companies({companyId})/users({userSecurityID})/userPermissions
```

**Response**

Here is an example of the response. 

> [!NOTE]  
>   The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

```json
{
    "userSecurityID": "82ae94d5-3445-47de-8668-714b5113a9c2",
    "id": "D365 EXTENSION MGT",
    "company": "",
    "scope": "System",
    "appID": "00000000-0000-0000-0000-000000000000",
    "displayName": "Dynamics 365-udvidelsesadmin.",
    "extensionName": ""
}
```

## See Also
[Working with [!INCLUDE[d365fin_long_md](../../includes/d365fin_long_md.md)] in Microsoft Graph](../resources/dynamics_overview.md)  
[Enabling the APIs for Microsoft Dynamics NAV](../../enabling-apis-for-dynamics-nav.md)  
[Endpoints for the APIs](../../endpoints-apis-for-dynamics.md)  
[Error Codes](../dynamics_error_codes.md)  
[UserPermission entity](../resources/dynamics_microsoft_automation_userPermission.md)  