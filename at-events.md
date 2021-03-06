---

copyright:
  years: 2016, 2021
lastupdated: "2021-06-03"

keywords: apps, event, security, activity tracker, applications, activity tracking events

subcollection: apps

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}
{:deprecated: .deprecated}
{:table: .aria-labeledby="caption"}

# {{site.data.keyword.dev_console}} {{site.data.keyword.cloudaccesstrailshort}} events
{: #at_events}

As a security officer, auditor, or manager, you can use the {{site.data.keyword.at_full}} to track how users and applications interact with the {{site.data.keyword.dev_console}} in the {{site.data.keyword.cloud}}.
{: shortdesc}

{{site.data.keyword.at_full_notm}} records user-initiated activities that change the state of a service in {{site.data.keyword.cloud_notm}}. You can use this service to investigate abnormal activity and critical actions, and to comply with regulatory audit requirements. In addition, you can receive alerts about actions as they happen. The events that are collected comply with the Cloud Auditing Data Federation (CADF) standard.

There are currently two {{site.data.keyword.at_full_notm}} services that are available in the {{site.data.keyword.cloud_notm}} catalog. The {{site.data.keyword.dev_console}} sends events to both services, and you can use either service to monitor the activity of the {{site.data.keyword.dev_console}}.

For more information, see [Getting started with {{site.data.keyword.at_full_notm}}](/docs/activity-tracker?topic=activity-tracker-getting-started).

## List of events
{: #at_actions}

The following table lists the actions that generate an event:

|Action	|Description	|
|-----|-------------|
|bluemix-developer-experience.app.create |An event is generated when a user creates an app.|
|bluemix-developer-experience.app.read |An event is generated when any of the following situations happen:<br><br>A user downloads the app code.<br><br>A user downloads the credentials file by using the {{site.data.keyword.dev_console}} CLI.<br><br>The {{site.data.keyword.cloud_notm}} infrastructure reads credentials for services that are associated with an app.<br><br>A user views the list of apps. For example, a user views the list of apps in the {{site.data.keyword.dev_console}} console or through the {{site.data.keyword.dev_cli_short}} (`ibmcloud dev`) commands in the {{site.data.keyword.cloud_notm}} Command Line Interface (CLI).|
|bluemix-developer-experience.app.update |An event is generated when any of the following situations happen:<br><br>Updates are made to the app. For example, a user modifies the name of the app.<br><br>A new service is created and added to an app.<br><br>An existing service is added to an app.<br><br>A service is removed from an app.<br><br>Code is generated for an app.<br><br>A DevOps toolchain is added through the {{site.data.keyword.cloud_notm}} console. For example, a user selects **Deploy your app** from the App details page.|
|bluemix-developer-experience.app.delete |An event is generated when a user deletes an app. |
{: caption="Table 1. Actions that generate events" caption-side="top"}

## Viewing events
{: #at_ui}

Events that are generated by an instance of the {{site.data.keyword.dev_console}} service are automatically forwarded to the {{site.data.keyword.at_full_notm}} service instance that is available in the same location.

{{site.data.keyword.at_full_notm}} can have only one instance per location. To view events, you must access the web UI of the {{site.data.keyword.at_full_notm}} service in the same location where your service instance is available. For more information, see [Manage access to the service](/docs/activity-tracker#gs_step2).

