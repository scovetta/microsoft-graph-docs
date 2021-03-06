---
title: "iosHomeScreenPage resource type"
description: "A page containing apps and folders on the Home Screen"
localization_priority: Normal
author: "tfitzmac"
ms.prod: "Intune"
---

# iosHomeScreenPage resource type

> **Important:** APIs under the /beta version in Microsoft Graph are subject to change. Use of these APIs in production applications is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

A page containing apps and folders on the Home Screen

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Name of the page|
|icons|[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection|A list of apps and folders to appear on a page. This collection can contain a maximum of 500 elements.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```




