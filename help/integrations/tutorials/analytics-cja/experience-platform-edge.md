---
title: Integrate Adobe [!DNL Analytics] and Customer Journey [!DNL Analytics] with the Experience [!DNL Platform] Edge tutorial
description: Learn how to integrate Adobe [!DNL Analytics] with Customer Journey [!DNL Analytics] using the AEP Web SDK, AEP Mobile SDK, or the Edge Network Server API.
solution: Customer Journey Analytics, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt: null
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integration" type="positive"
exl-id: e39dac5d-6ad5-47c8-94e8-070011233161
TQID: https://experienceleague.adobe.com/ClZddWXeWp51gWTBjRDQBZ2xNiO1bTRq-AoAdmucNEg
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
  - id: e98b7246-966c-4318-9e95-cad2f7a17dc7
    internal-label: Customer Journey Analytics
feature_v2:
  - id: b3f03848-ae12-48b2-8aab-cad18567eb32
    internal-label: Metrics
  - id: e75a4a9c-d354-4ca4-9b02-1afeca73fa5e
    internal-label: Integrations
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
    internal-label: Integrations
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
    internal-label: API
subfeature_v2:
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
    internal-label: Experience Cloud integration
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
---
# Integrate Adobe [!DNL Analytics] and Customer Journey [!DNL Analytics] with the Experience [!DNL Platform] Edge tutorial   

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Create schemas</a> for data to be ingested.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Create datasets</a> for data to be ingested.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configure the correct identities and identity namespaces on the schema</a> to be sure that the ingested data can stitch to a unified profile.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html" _target="_blank" rel="noopener noreferrer">Enable the schemas and datasets for profile</a>.</li>
    <li>Ingest data into Experience [!DNL Platform] using one of these methods:</li>
        <ul>
            <li>Experience [!DNL Platform] Web SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Checklist</a></li>
                </ul>
            <li>Experience [!DNL Platform] Mobile SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">Checklist</a></li>
                </ul></li>
            <li>Edge Network Server API:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><i>(Optional)</i>. If using multiple datasets, stitch the person ID's together to <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">generate a combined dataset</a>. If using a single [!DNL Analytics] dataset, or if a common identifier exists across all datasets you plan to use in Customer Journey [!DNL Analytics], skip this step.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html" _target="_blank" rel="noopener noreferrer">Create a connection</a> in Customer Journey [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Create a data view</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">configure the component settings</a>, and <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">format metrics</a> in Customer Journey [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html" _target="_blank" rel="noopener noreferrer">Create a project in Customer Journey [!DNL Analytics].</a></li>
</ol>                   

>[!NOTE]
>
>The standard workflow steps for the Adobe [!DNL Analytics] source connector create the schema and dataset used to ingest the data from [!DNL Analytics] "as-is". Therefore, the first two steps are handled by the system. The mapping workflow requires creating custom attributes; therefore, follow the sequence of steps fully.
