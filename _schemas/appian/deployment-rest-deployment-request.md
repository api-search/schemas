---
description: Request body for creating a deployment operation. For exports, provide the JSON configuration with export type and UUIDs. For imports, provide package files along with the JSON configuration.
layout: schema
name: DeploymentRequest
properties_list:
- description: JSON string containing the deployment configuration. For exports, includes exportType and uuids. For imports, includes name, description, and file name references.
  name: json
  type: string
- description: The deployment package ZIP file to import. Required for import operations.
  name: packageFileName
  type: string
- description: Admin Console settings ZIP file to import alongside the package.
  name: adminConsoleSettingsFileName
  type: string
- description: Import customization properties file that maps source environment values to target environment values.
  name: customizationFileName
  type: string
- description: Plug-ins ZIP file containing plug-ins to deploy.
  name: pluginsFileName
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-deployment-request-schema.json
slug: deployment-rest-deployment-request
source_filename: deployment-rest-deployment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-deployment-request-schema.json\",\n  \"title\": \"DeploymentRequest\",\n  \"description\": \"Request body for creating a deployment operation. For exports, provide the JSON configuration with export type and UUIDs. For imports, provide package files along with the JSON configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"json\": {\n      \"type\": \"string\",\n      \"description\": \"JSON string containing the deployment configuration. For exports, includes exportType and uuids. For imports, includes name, description, and file name references.\"\n    },\n    \"packageFileName\": {\n      \"type\": \"string\",\n      \"format\": \"binary\",\n      \"description\": \"The deployment package ZIP file to import. Required for import operations.\"\n    },\n    \"adminConsoleSettingsFileName\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"binary\",\n      \"description\": \"Admin Console settings ZIP file to import alongside the package.\"\n    },\n    \"customizationFileName\": {\n      \"type\": \"string\",\n      \"format\": \"binary\",\n      \"description\": \"Import customization properties file that maps source environment values to target environment values.\"\n    },\n    \"pluginsFileName\": {\n      \"type\": \"string\",\n      \"format\": \"binary\",\n      \"description\": \"Plug-ins ZIP file containing plug-ins to deploy.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-deployment-request-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: DeploymentRequest
---
