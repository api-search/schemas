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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-export-deployment-result-schema.json\",\n  \"title\": \"ExportDeploymentResult\",\n  \"description\": \"Result of an export deployment operation, including URLs to download the exported artifacts such as packages, plug-ins, customization files, and database scripts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"$ref\": \"#/components/schemas/DeploymentStatus\"\n    },\n    \"packageZip\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the exported package ZIP file.\"\n    },\n    \"dataSource\": {\n      \"type\": \"string\",\n      \"description\": \"The data source name or UUID associated with the export.\"\n    },\n    \"databaseScripts\": {\n      \"type\": \"array\",\n      \"description\": \"Array of database\
  \ script objects included in the export.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DatabaseScript\"\n      }\n    },\n    \"pluginsZip\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the exported plug-ins ZIP file.\"\n    },\n    \"customizationFile\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the export customization file.\"\n    },\n    \"customizationFileTemplate\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download a template customization file for the exported package.\"\n    },\n    \"deploymentLogUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to retrieve the full deployment log.\"\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-export-deployment-result-schema.json
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
