---
title: "Monitor the Appliance by Using System Center Operations Manager (Analytics Platform System)"
ms.custom: na
ms.date: 07/27/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: de6cbf6e-f2e9-4877-94df-9c13b1182d56
caps.latest.revision: 14
author: BarbKess
---
# Monitor the Appliance by Using System Center Operations Manager (Analytics Platform System)
This describes how to use System Center Operations Manager to monitor SQL Server PDW and HDInsight.  
  
Parent Topic: [Appliance Management Tasks &#40;Analytics Platform System&#41;](../management/appliance-management-tasks-analytics-platform-system.md)  
  
## Before You Begin  
  
### Prerequisites  
  
1.  System Center Operations Manager 2007 R2, 2012, or 2012 SP1 must be installed and running.  
  
2.  SQL Server 2008 R2 Native Client or SQL Server 2012 Native Client must be installed.  
  
3.  The management packs to monitor SQL Server PDW and HDInsight must be installed, imported, and configured. Use the following for instructions to perform these tasks.  
  
    -   [Install the SCOM Management Packs &#40;Analytics Platform System&#41;](../management/install-the-scom-management-packs-analytics-platform-system.md)  
  
    -   [Import the SCOM Management Pack for PDW &#40;Analytics Platform System&#41;](../management/import-the-scom-management-pack-for-pdw-analytics-platform-system.md)  
  
    -   [Import the SCOM Management Pack for HDInsight &#40;Analytics Platform System&#41;](../management/import-the-scom-management-pack-for-hdinsight-analytics-platform-system.md)  
  
    -   [Configure SCOM to Monitor Analytics Platform System &#40;Analytics Platform System&#41;](../management/configure-scom-to-monitor-analytics-platform-system-analytics-platform-system.md)  
  
## To Monitor SQL Server PDW with SCOM  
After configuring the SCOM Management Packs, click on the Monitoring Pane of SCOM and drill down to **SQL Server Appliance** and then **Microsoft SQL Server Parallel Data Warehouse**. Underneath Microsoft SQL Server Parallel Data Warehouse, there are four choices: Alerts, Appliances, Appliance Diagram, and nodes.  
  
### Alerts  
Alerts are where you can find the current alerts to manage.  
  
![Alerts](../management/media/SCOM_SCOM.png "SCOM_SCOM")  
  
### Appliances  
Appliances are where you will find the currently discovered and monitored SQL Server PDW Appliances in your environment. If an appliance does not show up here and you have created the ODBC connection for it, then there may be something wrong with your PDWWatcher account. If they show up as “Not monitored” there may be something wrong with your PDWMonitor account. Please be patient as SCOM does not make changes in real time, but periodically checks for new appliances to monitor and periodically sends queries to appliances for monitoring.  
  
![Appliances](../management/media/SCOM_SCOM2.png "SCOM_SCOM2")  
  
### Appliances Diagram  
The Appliances Diagram Page is where you can get a look at the health of your appliance with a tree view:  
  
![Appliances diagram](../management/media/SCOM_SCOM3.png "SCOM_SCOM3")  
  
### Nodes  
Finally, the Nodes view allows you to see the health of your appliance through each node:  
  
![Nodes](../management/media/SCOM_SCOM4.png "SCOM_SCOM4")  
  
## See Also  
[Common Metadata Query Examples &#40;SQL Server PDW&#41;](../sqlpdw/common-metadata-query-examples-sql-server-pdw.md)  
[Understanding Admin Console Alerts &#40;Analytics Platform System&#41;](../management/understanding-admin-console-alerts-analytics-platform-system.md)  
  