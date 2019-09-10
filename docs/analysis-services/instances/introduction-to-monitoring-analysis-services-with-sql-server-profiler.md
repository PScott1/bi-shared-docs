---
title: "Monitoring Analysis Services with SQL Server Profiler | Microsoft Docs"
ms.date: 09/05/2019
ms.prod: sql
ms.technology: analysis-services
ms.custom:
ms.topic: conceptual
ms.author: owend
ms.reviewer: owend
author: minewiskan
manager: kfile
---
# Monitoring Analysis Services with SQL Server Profiler

[!INCLUDE[ssas-appliesto-sqlas-all-aas-pbip](../../includes/ssas-appliesto-sqlas-all-aas-pbip.md)]

  You can use SQL Server Profiler to monitor events generated by an instance of Analysis Service to do the following:  
  
-   Monitor the performance of an instance of the Analysis Services engine.  
  
-   Debug query statements.  
  
-   Identify queries that run slowly.  
  
-   Test query statements in the development phase of a project by stepping through statements to confirm that the code works as expected.  
  
-   Troubleshoot problems by capturing events on a production system and replaying them on a test system. This approach is useful for testing or debugging purposes and lets users continue to use the production system without interference.  
  
-   Audit and review activity that occurred on an instance. A security administrator can review any one of the audited events. This includes the success or failure of a login try and the success or failure of permissions in accessing statements and objects.  
  
-   Display data about the captured events to the screen, or capture and save data about each event to a file or [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] table for future analysis or playback. When you replay data, you can rerun the saved events as they originally occurred, either in real time or step by step.  
  
## Using SQL Server Profiler

 To use SQL Server Profiler to create or replay traces, you must be a member of the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] server role. If you are a member of the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] server role, you can start SQL Server Profiler from the [!INCLUDE[msCoName](../../includes/msconame-md.md)] [!INCLUDE[ssNoVersion](../../includes/ssnoversion-md.md)] program group on the **Start** menu.  
  
 When you use SQL Server Profiler, note the following:  
  
-   Trace definitions are stored with the [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] database by using the CREATE statement.  
  
-   Multiple traces can be running at the same time.  
  
-   Multiple connections can receive events from the same trace.  
  
-   A trace can continue when [!INCLUDE[ssASnoversion](../../includes/ssasnoversion-md.md)] stops and restarts.  
  
    > [!NOTE]  
    >  Passwords are not revealed in trace events, but are replaced by \*\*\*\*\*\* in the event.  
  
 For optimal performance, use SQL Server Profiler to monitor only those events in which you are most interested. Monitoring too many events adds overhead and can cause the trace file or table to grow very large, especially when you monitor over a long period of time. In addition, use filtering to limit the amount of data that is collected and to prevent traces from becoming too large.  
  
## See Also  
 [Analysis Services Trace Events](https://docs.microsoft.com/bi-reference/trace-events/analysis-services-trace-events)   
 [Create Profiler Traces for Replay &#40;Analysis Services&#41;](../../analysis-services/instances/create-profiler-traces-for-replay-analysis-services.md)  
  
  