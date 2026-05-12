---
title: Integrate [!DNL Analytics] and Real-Time Customer Data [!DNL Platform] with Experience [!DNL Platform] source connector tutorial
description: Learn how to integrate Adobe [!DNL Analytics] with Real-Time Customer Data [!DNL Platform] using the Experience [!DNL Platform] source connector.
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integration" type="positive"
exl-id: 1e27555d-e609-4a04-91ca-9518898ad699
TQID: https://experienceleague.adobe.com/Uct30-UadP-2Ocwslbk-dMAV0Y2unZlA339hThnofpA
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
feature_v2:
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
    internal-label: Integrations
subfeature_v2:
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
    internal-label: Experience Cloud integration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
---
# Integrate Adobe [!DNL Analytics] and Real-Time Customer Data [!DNL Platform] with Experience [!DNL Platform] source connector

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Create schemas</a> for data to be ingested.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Create datasets</a> for data to be ingested.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Configure the correct identities and identity namespaces on the schema</a> to be sure that the ingested data can stitch to a unified profile.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html" _target="_blank" rel="noopener noreferrer">Enable the schemas and datasets for profile</a>.</li>
    <li>Ingest [!DNL Analytics] data into Experience platform using the <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] source connector</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">Create segments in Experience [!DNL Platform].</a> The system automatically determines whether the segment is evaluated as batch (data connector) or streaming (Edge network).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Configure destinations for sharing of profile attributes and audience memberships to desired destinations.</a></li>   
</ol>                   

>[!NOTE]
>
>The standard workflow steps for the Adobe [!DNL Analytics] source connector create the schema and dataset used to ingest the data from [!DNL Analytics] "as-is". Therefore, the first two steps are handled by the system. The mapping workflow requires creating custom attributes; therefore, follow the sequence of steps fully.
