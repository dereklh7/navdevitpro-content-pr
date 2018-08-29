---
title: complex types JSON | Microsoft Docs
description: Complex data types in JSON for Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen

ms.service: dynamics365-businesscentral
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 03/19/2018
ms.author: solsen
---

# complex types JSON
These are the various complex types in Dynamics 365 Business Central. You can see usage of these complex types in the various individual methods that make use of them.

## Postal address

Represents a Postal Address complex type in Dynamics 365 Business Central.       

### Properties
| Property	   | Type	    |Description             |
|:-------------|:---------|:-----------------------|
|street        |string    |Postal address street.  |
|city          |string    |Postal address city.    |
|state         |string    |Postal address state.   |
|countryLetterCode|string |Postal address country letter code (two character word)|
|postalCode    |string    |Postal address post code|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```

## See also
[Working with Dynamics 365 Business Central in Microsoft Graph](../resources/dynamics_overview.md)  
[Error Codes](../dynamics_error_codes.md)  