---
title: Integrate [!DNL Analytics] with [!DNL Commerce] tutorial
description: Learn how to integrate [!DNL Analytics] with [!DNL Commerce].
solution: Analytics, Commerce
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integration" type="positive"
exl-id: ef50b6b3-1e2b-4fe9-98d5-555bc14ae8d6
TQID: https://experienceleague.adobe.com/yG4EZoiPmm3-HnjD6lZCyBDpaeseNuGb5wRhnCWqRuk
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
  - id: eadea719-cf89-469b-a6fd-a236a7138047
    internal-label: Commerce
feature_v2:
  - id: c153fd90-23e1-4614-81d3-3cc7571227f7
    internal-label: Analysis Workspace
  - id: c32adafa-ed01-4b31-997e-2413013911b0
    internal-label: Integrations
  - id: dac87252-6066-4d6e-a9d2-f6d84c323de7
    internal-label: Configuration
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
    internal-label: Integrations
subfeature_v2:
  - id: dcae653e-62c6-4cc8-84e6-ee110b848296
    internal-label: Visualizations
  - id: e318d41c-1d01-4c1e-9b18-1f61d435ceee
    internal-label: Freeform tables
  - id: e38cbddc-1633-4cd5-bed5-9f289f2a6029
    internal-label: Panels
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
    internal-label: Experience Cloud integration
  - id: ef60b66e-5984-4336-ba72-6d978b1b6f87
    internal-label: Report suites
  - id: f236e2a1-90d4-477d-92e1-5996b5e92bff
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
topic_v2:
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
---
# Integrate [!DNL Analytics] with [!DNL Commerce]

## Initial Onboarding

These instructions are for Adobe [!DNL Commerce] Cloud hosted projects. Self-hosted can vary to some degree, but the overall process should be similar.

1. Check out the code in your local environment
1. Use composer and install module
1. Follow the individual instructions here and return when completed to finish the remaining steps
    [Install and configure the Experience [!DNL Platform] connector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. Commit the composer.json and if on cloud, composer.lock files
1. Verify that module is on the staging and/or production environments 
    You can do this by logging into the admin section of Adobe [!DNL Commerce] and looking for these new sections under System > Services
    ![Experience [!DNL Platform] connector extension](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Configure the module with your credentials from inside the Adobe [!DNL Commerce] back office.
    * First the [!DNL Commerce] Services connector configurations, as shown below.
![[!DNL Commerce] Services Connector Setup](./assets/analytics-commerce/commerce-services-connector-setup.png)
    * Then the Experience [!DNL Platform] connector settings, as shown below.
![Experience [!DNL Platform] connector](./assets/analytics-commerce/experience-platform-connector.png)

For greater details on each phase and step of the onboarding process, follow the instructions on the [Experience [!DNL Platform] connector overview](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}. The Experience [!DNL Platform] connector tutorial covers each section in depth and answer any questions you may have. Use this tutorial for the rest of the quick setup steps.

## Configuration of Experience Edge and Adobe [!DNL Analytics]

1. Verify that your organization has (and you have) access to Adobe [!DNL Analytics]. This can be confirmed by going to the [Adobe Experience Cloud homepage](https://experience.adobe.com/) and clicking on the application switcher (nine dots) in the top navigation.  

1. Create a new report suite in Adobe [!DNL Analytics], or identify the ID of the report suite that you will be pushing [!DNL Commerce] data into. For more info, watch a tutorial on [creating a new report suite](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html). You will need this report suite ID in the datastream step below.

1. Navigate to the [Adobe Experience [!DNL Platform] interface](https://platform.adobe.com) if you have access to Experience [!DNL Platform]. If you don't have access to that interface, you can perform all necessary steps listed below in the Adobe Experience [!DNL Platform] [Data Collection interface](https://experience.adobe.com/#/data-collection).

1. Create or update your XDM schema with [!DNL Commerce]-specific field groups. For more information on how to create a schema, please see the ["Create schemas"](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html) tutorial.  
    * You will need to select this schema from the options in the datastream step below. To create a schema, Look in the left column under **Data Management** and find **Schemas**. Now on the top right of the interface, click **Create schema**. Select XDM ExperienceEvent.
    * After creating a new schema, you will add the [!DNL Commerce] field groups. On the left side of the UI, find Field groups, and click **Add**
        * In the search, you can filter by entering `ExperienceEvent Commerce`
        * Select the **Adobe [!DNL Analytics] ExperienceEvent [!DNL Commerce]** by checking the box
        * Then click **Add field groups** on the top right to save and continue

1. Optionally (and only if you are in the Experience [!DNL Platform] interface) - Create a new dataset
    * This step allows you to bring the [!DNL Commerce] data into the Experience [!DNL Platform] (separately from bring the data into Adobe [!DNL Analytics]). Do this step if you have access to Experience [!DNL Platform], and are planning to use the [!DNL Commerce] data in the Experience [!DNL Platform]-supported applications, like Real-Time Customer Data [!DNL Platform], Customer Journey [!DNL Analytics], or Journey Optimizer.   
    * You will need to select this dataset from the options in the datastream step below.
    * Under the left column **Data Management** heading in the left navigation, select **Datasets**.  
    * Click **Create dataset** in the top right. Choose the **Create dataset from schema** option.  
    * Search for and use the schema that you created in the last step

1. Create the Datastream to send the [!DNL Commerce] data to Adobe [!DNL Analytics]
    * Under the **Data Collection** heading in the left column, select **Datastreams**.
    * Click **New Datastream** on the top right of the interface.
    * Provide a name and and optional description.
    * Find and select the schema that you created/identified in the previous step.
    * Add any desired advanced options. For more information about the advanced options, please visit the [documentation](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html).
    * Click **Save** to continue.
    * Click **Add Service** and choose **Adobe [!DNL Analytics]** in the drop-down field.
    * Click **Add Report Suite** and enter the report suite ID that you created/identified in a previous step. You can add more than one report suite if you would like the data to flow into multiple report suites.
    * Optionally, and if you created a dataset in a previous step, click **Add Service** again, choosing **Adobe Experience [!DNL Platform]** from the drop-down field. In the Event Dataset field, select the dataset that you previously created.
    * Save the Datastream.

1. Finally, to view your [!DNL Commerce] data, you will need to navigate to Analysis Workspace in Adobe [!DNL Analytics], create a project, choose your report suite, and add freeform tables and other visualizations to report on and analyze your [!DNL Commerce] data. The following image shows one example of a table you can create in Analysis Workspace.

    ![[!DNL Analytics] Screenshot of some commerce data](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

    Here are some additional resources to help you work in Analysis Workspace:

    * [Analysis Workspace overview](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
    * [Building a Workspace project from scratch](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
    * [Using Tables, Visualizations, and Panels in Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
    * [Visualization use cases](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

    Additionally, there are free courses available on Experience League. See [!DNL Analytics] courses available [HERE](https://experienceleague.adobe.com/?lang=en&Solution=Analytics#courses).
