---
description: Configuration for an import deployment operation specifying the files and settings to deploy.
layout: schema
name: ImportConfiguration
properties_list:
- description: Name of the deployment, displayed in Appian Designer's Deploy view.
  name: name
  type: string
- description: Description of the deployment.
  name: description
  type: string
- description: File name of the deployment package ZIP file attached in the form data.
  name: packageFileName
  type: string
- description: File name of the Admin Console settings ZIP file attached in the form data.
  name: adminConsoleSettingsFileName
  type: string
- description: File name of the import customization properties file attached in the form data.
  name: customizationFileName
  type: string
- description: File name of the plug-ins ZIP file attached in the form data.
  name: pluginsFileName
  type: string
- description: The data source name or UUID for database script execution.
  name: dataSource
  type: string
- description: Array of database script configurations specifying file names and execution order.
  name: databaseScripts
  type: array
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-import-configuration-schema.json
slug: deployment-rest-import-configuration
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: ImportConfiguration
---
