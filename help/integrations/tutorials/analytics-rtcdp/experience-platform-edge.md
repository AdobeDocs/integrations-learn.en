---
title: Integrate [!DNL Analytics] and Real-Time Customer Data [!DNL Platform] with the Experience [!DNL Platform] Edge tutorial
description: Learn how to integrate Adobe [!DNL Analytics] with Real-Time Customer Data [!DNL Platform] using the AEP Web SDK, AEP Mobile SDK, or the Edge Network Server API.
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt: 13732
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integration" type="positive"
exl-id: 07c2c329-0810-4f66-a91a-e315695f3fb4
TQID: https://experienceleague.adobe.com/K1CpRtUekl5jQNDMGswJpexC9fv9uVmgraLlNFXUIr8
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
feature_v2:
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
# Integrate Adobe [!DNL Analytics] and Real-Time Customer Data [!DNL Platform] with Experience [!DNL Platform] Edge tutorial

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
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html" _target="_blank" rel="noopener noreferrer">Create segments in Experience [!DNL Platform].</a> The system automatically determines whether the segment is evaluated as batch (data connector) or streaming (Edge network).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Configure destinations for sharing of profile attributes and audience memberships to desired destinations.</a></li>
</ol>

>[!NOTE]
>
>The standard workflow steps for the Adobe [!DNL Analytics] source connector create the schema and dataset used to ingest the data from [!DNL Analytics] "as-is". Therefore, the first two steps are handled by the system. The mapping workflow requires creating custom attributes; therefore, follow the sequence of steps fully.
