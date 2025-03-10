---
title: Transportation management overview
description: Access an overview of the transportation management functionality in Supply Chain Management, including a table outlining information for various scenarios.
author: lisascholz
ms.author: lisascholz
ms.topic: overview
ms.date: 05/22/2024
ms.custom: 
  - bap-template
ms.reviewer: kamaybac
ms.search.form: TMSParameters,TMSRateRouteWorkbench, WHSLoadPlanningWorkbench, WHSInboundLoadPlanningWorkbench, WHSOutboundLoadPlanningWorkbench, TMSLoadBuildTemplateApply, WHSLoadTemplate, TMSTransportationStatus, TMSLoadSeal, TMSLoadBuildProposal, TMSLoadBuildWorkbench, TMSLoadBuildStrategy, TMSLoadBuildStrategyAttributeValue
---

# Transportation management overview

[!include [banner](../includes/banner.md)]

This article gives an overview of the transportation management functionality in Supply Chain Management.

Transportation management lets you use your company’s transportation, and also lets you identify vendor and routing solutions for inbound and outbound orders. For example, you can identify the fastest route or the least expensive rate for a shipment. The following table describes the main scenarios for using Transportation management.

| Scenario | How Transportation management can help |
|---|---|
| Use external logistics providers for transportation activities. | Use Transportation management for inbound and/or outbound transportation. |
| The company's own fleet is available for delivery/pickup, and delivery charges are passed on to customers. | For the outbound processes, you can use Transportation management to determine the transportation charges and pass them on to customers. However, the carrier invoice reconciliation process isn't required. |
| The company's own fleet is available for delivery/pickup, but delivery charges aren't passed on to customers, because product prices include transportation. | Many of the settings and features of Transportation management aren't required. However, you can use Transportation management to determine the transportation rates and adjust the sales price accordingly. |
| Logistics service is provided by another legal entity in the same company. | You can use Transportation management by treating the other legal entity like any other shipping carrier. You can't automate the economic transactions between legal entities. Therefore, you must handle these transactions manually (for example, by creating a purchase order).<br><br>In the legal entity that provides the logistics services, Transportation management can be used to determine transportation rates. |

## Planning transportation in Supply Chain Management

In Transportation management, transportation planning can be based either on orders or on the shipments that are created based on those orders. The shipments always exist at some point in time but aren't required for transportation planning. Transfer orders are part of the outbound scenario and can be planned together with sales orders.

![Load drawing.](./media/Load-drawing1-1024x477.jpg)

## Inbound transportation

When you order items from a vendor, and the items must be delivered to your warehouse, you might want to arrange the transport of the items yourself. You can use Supply Chain Management to plan the transportation and receipt of the inbound load. The following illustration shows the business process flow for planning transportation for an inbound load.

![Business process flow for inbound load transportation.](./media/Businessprocessflowforinboundloadtransportation.jpg)

## Outbound transportation

You can plan and process an outbound load to ship specific items from a company’s warehouse to a customer. You can use Supply Chain Management to plan the transportation and shipping of an outbound load. The following illustration shows the business process flow for planning and processing outbound loads for shipping.

![Planning and processing outbound loads.](./media/Planningandprocessingoutboundloads.jpg)

## Load building

Supply Chain Management provides a load building strategy that is named the Volume-based load building strategy. This strategy lets you use the maximum values that are specified for height and weight in the load template, or you can override the settings by entering new values. To use this strategy, select it in the **Load building strategy** field on the **Setup** FastTab on the **Load building workbench** page. In addition, you can add your own load-building strategies by creating a new class in the Application Object Tree (AOT).

## White papers

The following white papers explore various aspects of transportation management in Dynamics 365 Supply Chain Management:

- [Transportation management engines](https://download.microsoft.com/download/e/0/9/e0957665-c12f-43c7-94c0-611cc49d7d61/TransportationManagementEnginesInAX.pdf)
- [Implementing and deploying Transportation management engines](https://download.microsoft.com/download/b/5/f/b5ff8fef-3918-4c1d-92d5-b67eb0971684/ImplementingAndDeployingTransportationManagementEnginesInAX.pdf)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
