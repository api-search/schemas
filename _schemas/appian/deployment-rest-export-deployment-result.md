---
description: Result of an export deployment operation, including URLs to download the exported artifacts such as packages, plug-ins, customization files, and database scripts.
layout: schema
name: ExportDeploymentResult
properties_list:
- description: ''
  name: status
  type: object
- description: URL to download the exported package ZIP file.
  name: packageZip
  type: string
- description: The data source name or UUID associated with the export.
  name: dataSource
  type: string
- description: Array of database script objects included in the export.
  name: databaseScripts
  type: array
- description: URL to download the exported plug-ins ZIP file.
  name: pluginsZip
  type: string
- description: URL to download the export customization file.
  name: customizationFile
  type: string
- description: URL to download a template customization file for the exported package.
  name: customizationFileTemplate
  type: string
- description: URL to retrieve the full deployment log.
  name: deploymentLogUrl
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-export-deployment-result-schema.json
slug: deployment-rest-export-deployment-result
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: ExportDeploymentResult
---
