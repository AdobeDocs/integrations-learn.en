---
title: Integrate [!DNL Analytics] and Customer Journey [!DNL Analytics] with Experience [!DNL Platform] source connector tutorial
description: Learn how to integrate Adobe [!DNL Analytics] with Customer Journey [!DNL Analytics] using the Experience [!DNL Platform] source connector.
solution: Customer Journey Analytics, Target
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13727
thumbnail: null
last-substantial-update: 2023-04-11
badgeIntegration: label="Integration" type="positive"
exl-id: f0dbd59d-d5e5-40e6-b4a4-e4789e7dd7e3
---
# Integrate Adobe [!DNL Analytics] and Customer Journey [!DNL Analytics] with Experience [!DNL Platform] source connector    

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Create schemas</a> for data to be ingested.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Create datasets</a> for data to be ingested.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configure the correct identities and identity namespaces on the schema</a> to be sure that the ingested data can stitch to a unified profile.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html" _target="_blank" rel="noopener noreferrer">Enable the schemas and datasets for profile</a>.</li>
    <li>Ingest data into Experience [!DNL Platform] using the <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] source connector</a></li>
    <li><i>(Optional)</i>. If using multiple datasets, stitch the person ID's together to <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">generate a combined dataset</a>. If using a single [!DNL Analytics] dataset, or if a common identifier exists across all datasets you plan to use in Customer Journey [!DNL Analytics], skip this step.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html" _target="_blank" rel="noopener noreferrer">Create a connection</a> in Customer Journey [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Create a data view</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">configure the component settings</a>, and <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">format metrics</a> in Customer Journey [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html" _target="_blank" rel="noopener noreferrer">Create a project in Customer Journey [!DNL Analytics].</a></li>
</ol>                   

>[!NOTE]
>
>The standard workflow steps for the Adobe [!DNL Analytics] source connector create the schema and dataset used to ingest the data from [!DNL Analytics] "as-is". Therefore, the first two steps are handled by the system. The mapping workflow requires creating custom attributes; therefore, follow the sequence of steps fully.
