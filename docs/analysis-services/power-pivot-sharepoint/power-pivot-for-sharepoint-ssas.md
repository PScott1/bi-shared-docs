---
title: "Power Pivot for SharePoint (SSAS) | Microsoft Docs"
ms.date: 09/10/2019
ms.prod: sql
ms.technology: analysis-services
ms.custom: ppvt-sharepoint
ms.topic: conceptual
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
---
# Power Pivot for SharePoint (SSAS)

[!INCLUDE[ssas-appliesto-sqlas](../../includes/ssas-appliesto-sqlas.md)]
  
Analysis Services in Power Pivot mode provides server hosting of Power Pivot data in a SharePoint farm. Power Pivot data is an analytical data model users create with Power Pivot in Excel.  
  
Server hosting of workbooks requires SharePoint, Excel Services, and an installation of Power Pivot for SharePoint. Data is loaded on Power Pivot for SharePoint instances where it can be refreshed at scheduled intervals using the Power Pivot data refresh capability.
  
## Power Pivot for SharePoint 2019

Support for Power Pivot Gallery and Refresh was removed from SharePoint Server 2019, effectively ending Analysis Services Power Pivot for SharePoint support for SharePoint 2019 and later. To learn more, see [What's deprecated or removed from SharePoint Server 2019](
https://docs.microsoft.com/sharepoint/what-s-new/what-s-deprecated-or-removed-from-sharepoint-server-2019#removed-features-in-sharepoint-server-2019). 

## Power Pivot for SharePoint 2016

SQL Server 2019, 2017, 2016 Analysis Services Power Pivot for SharePoint mode supports SharePoint 2016 and Office Online Server usage of Excel workbooks containing data models and Reporting Services Power View reports.
  
Excel, within Office Online Server includes data model functionality to enable interaction with a Power Pivot workbook in the browser. You do not need to deploy the Power Pivot for SharePoint 2016 add-in into the farm. You only need to install an Analysis Services server in Power Pivot mode and register the server with Office Online Server.  
  
Deploying the Power Pivot for SharePoint 2016 add-in enables additional functionality and features in your SharePoint farm. The additional features include Power Pivot Gallery and Schedule Data Refresh.  
  
 ![SSAS Power Pivot Mode 3 Server with Office Online Server](../../analysis-services/power-pivot-sharepoint/media/as-powerpivot-mode-3server-oos-deploy.png)  
  
## Power Pivot for SharePoint 2013

SQL Server 2017 Power Pivot for SharePoint supports Microsoft SharePoint 2013 Excel Services usage of Excel workbooks containing data models and Reporting Services Power View reports.
  
Excel Services in SharePoint 2013 includes data model functionality to enable interaction with a Power Pivot workbook in the browser. You do not need to deploy the Power Pivot for SharePoint 2013 add-in into the farm. You only need to install an Analysis Services server in SharePoint mode and register the server within the Excel Services **Data Model** settings.  
  
 Deploying the Power Pivot for SharePoint 2013 add-in enables additional functionality and features in your SharePoint farm. The additional features include Power Pivot Gallery, Schedule Data Refresh, and the Power Pivot Management Dashboard.  
  
 ![SSAS PowerPivot Mode 2 Server Deployment](../../analysis-services/power-pivot-sharepoint/media/as-powerpivot-mode-2server-deployment.gif "SSAS PowerPivot Mode 2 Server Deployment")