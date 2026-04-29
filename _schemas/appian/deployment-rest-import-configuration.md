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
source_filename: deployment-rest-import-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-import-configuration-schema.json\",\n  \"title\": \"ImportConfiguration\",\n  \"description\": \"Configuration for an import deployment operation specifying the files and settings to deploy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the deployment, displayed in Appian Designer's Deploy view.\",\n      \"example\": \"Q4 Release Package\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the deployment.\"\n    },\n    \"packageFileName\": {\n      \"type\": \"string\",\n      \"description\": \"File name of the deployment package ZIP file attached in the form data.\"\n    },\n    \"adminConsoleSettingsFileName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"File name of the Admin Console settings ZIP file attached in the form data.\"\n    },\n    \"customizationFileName\": {\n      \"type\": \"string\",\n      \"description\": \"File name of the import customization properties file attached in the form data.\"\n    },\n    \"pluginsFileName\": {\n      \"type\": \"string\",\n      \"description\": \"File name of the plug-ins ZIP file attached in the form data.\"\n    },\n    \"dataSource\": {\n      \"type\": \"string\",\n      \"description\": \"The data source name or UUID for database script execution.\"\n    },\n    \"databaseScripts\": {\n      \"type\": \"array\",\n      \"description\": \"Array of database script configurations specifying file names and execution order.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fileName\": {\n            \"type\": \"string\",\n            \"description\": \"The file name of the database script.\"\n          },\n          \"orderId\": {\n     \
  \       \"type\": \"string\",\n            \"description\": \"The execution order for the script, starting at 1.\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-import-configuration-schema.json
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
