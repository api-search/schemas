---
description: Configuration for an export deployment operation specifying what to export and how.
layout: schema
name: ExportConfiguration
properties_list:
- description: Specifies the kind of export being performed. Use package for a single package or application for one or more applications.
  name: exportType
  type: string
- description: Array of UUIDs to export. For packages, provide a single UUID. For applications, provide one or more application UUIDs.
  name: uuids
  type: array
- description: Custom name for the deployment. If omitted, a name is auto-generated.
  name: name
  type: string
- description: Description of the deployment, displayed in Appian Designer.
  name: description
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-export-configuration-schema.json
slug: deployment-rest-export-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-export-configuration-schema.json\",\n  \"title\": \"ExportConfiguration\",\n  \"description\": \"Configuration for an export deployment operation specifying what to export and how.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportType\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the kind of export being performed. Use package for a single package or application for one or more applications.\",\n      \"enum\": [\n        \"package\",\n        \"application\"\n      ]\n    },\n    \"uuids\": {\n      \"type\": \"array\",\n      \"description\": \"Array of UUIDs to export. For packages, provide a single UUID. For applications, provide one or more application UUIDs.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      },\n\
  \      \"minItems\": 1\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Custom name for the deployment. If omitted, a name is auto-generated.\",\n      \"example\": \"CR-176543 Add reports dashboard\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the deployment, displayed in Appian Designer.\",\n      \"example\": \"Updates the executive summary view.\"\n    }\n  },\n  \"required\": [\n    \"exportType\",\n    \"uuids\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-export-configuration-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: ExportConfiguration
---
