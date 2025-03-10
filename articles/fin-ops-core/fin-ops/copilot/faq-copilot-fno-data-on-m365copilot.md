---
title: Responsible AI FAQ for Chat with finance and operations data on Microsoft 365 Copilot
description: This FAQ provides information about the AI technology used in Chat with finance and operations data on Microsoft 365 Copilot, along with key considerations and details about how AI is used, how it was tested and evaluated, and any specific limitations.
ms.date: 10/04/2024
ms.custom: 
  - responsible-ai-faqs
ms.topic: article
author: RamaKrishnamoorthy
ms.author: ramasri
ms.reviewer: johnmichalak
---

# Responsible AI FAQ for Chat with finance and operations data on Microsoft 365 Copilot

These frequently asked questions (FAQ) describe the AI impact of the *Chat with finance and operations data on Microsoft 365 Copilot* feature in finance and operations apps.

## What is Chat with finance and operations data on Microsoft 365 Copilot?

This feature lets you use Microsoft 365 Copilot to chat with finance and operations data through virtual entities in Dataverse.

## What are the capabilities of Chat with finance and operations data on Microsoft 365 Copilot?

This feature provides a guided conversational experience that helps you quickly identify available inventory in finance and operation apps without having to leave the work context in Microsoft 365.

## What is the intended use of Chat with finance and operations data on Microsoft 365 Copilot?

A Microsoft 365 Copilot license enables authorized users to engage in a natural-language conversation with finance and operations data. For example, they can ask the following questions:

- I need 6 Southridge Video Laptop16 M1601 in Silver color and 5 Laptop15 M1501 in Red color. Can you check the availability? Give me the details by product name, site, warehouse, color, available quantity.
- Do we have red Laptop15 M1501 model in warehouses other than Chicago within the site Central? Give me the details by product name, site, warehouse, color, available quantity.

Microsoft 365 Copilot is based on the data that resides inside finance and operation apps and responds to users.

The intended users are Microsoft 365 Copilot users who have the security role and privileges that are required to access the related querying data in Dynamics 365 Supply Chain Management (for example, on-hand inventory data).

## How was Chat with finance and operations data on Microsoft 365 Copilot evaluated? What metrics are used to measure performance?

The evaluation of Chat with finance and operations data on Microsoft 365 Copilot involved a multi-phase testing process to ensure its accuracy and reliability. The key components of the evaluation included:

1. **Golden Tests**: A series of predefined test cases, known as golden tests, were conducted to simulate real-world scenarios where users interact with financial and operations data. These test cases are designed to cover a wide range of common use cases and ensure that the Copilot feature responds accurately and efficiently.

2. **Test Automation**: To maintain consistency and monitor performance over time, these golden test cases were integrated into an automated testing suite. This allows the team to run regular checks and ensure that updates or changes to the system don’t introduce new issues or regressions.

3. **Performance Metrics**: Several metrics are used to measure the performance of the feature:
   - **Accuracy of Responses**: The primary metric is the accuracy of the Copilot's responses, especially regarding inventory levels and data queries.
   - **Response Time**: The speed at which Copilot responds to user queries is measured to ensure that it delivers information in real-time or within an acceptable time frame.
   - **User Satisfaction**: Feedback from pilot users and testers is gathered to assess the usability and helpfulness of the feature.
   - **Error Rate**: The frequency of incorrect or incomplete responses is monitored to identify areas that need improvement.
     
By combining automated testing with real-world usage feedback and rigorous performance metrics, Microsoft ensures that Chat with finance and operations data on Microsoft 365 Copilot meets high standards for accuracy, speed, and reliability.

## What are the limitations of Chat with finance and operations data on Microsoft 365 Copilot? How can users minimize the impact of these limitations when they use the system?

When the feature doesn't work as intended, it provides inaccurate inventory quantities and can negatively affect the customer's business. Here are some examples of the impacts:

- **Lost sales** – If Copilot responds with more stock than Supply Chain Management on-hand inventory records, especially in a stock-out scenario, the inaccurate inventory availability might cause sales manager to lose potential customers.
- **Wasted resources** – If Copilot responds with an inaccurate inventory amount, the inaccuracy might cause overstocking of products.
- **Poor customer satisfaction** – If Copilot's response is inaccurate, the inaccuracy might cause a failure to deliver orders on time. Therefore, it might lead to customer dissatisfaction and lower retention rates.
- **Insufficient inventory management** – If Copilot's response is inaccurate, the inaccuracy might cause poor inventory management and unnecessary inventory transfers between locations. Therefore, it might increase the risk of understocking or overstocking in different warehouses.

Users can help minimize these impacts by using only the prompts that are documented in the documentation.

## What operational factors and settings allow for effective and responsible use of the feature?

With an understanding of the potential negative impact, Microsoft plans to implement the following mitigations:

- We're fixing the plugin invocation pipeline to improve the hit ratio and increase the probability that the plugin is invoked based on user utterances.
- We're developing a more advanced and stable concept that is known as *knowledge*. The plugin must be upgraded to knowledge at some point after it becomes ready for consumption.

## See also

- [Chat with finance and operations data on Microsoft 365 Copilot](../../dev-itpro/m365-copilot/chat-with-fno-data-on-m365copilot.md)
