---
description: ''
layout: schema
name: ExtensionUpload
properties_list:
- description: ''
  name: systemId
  type: string
- description: When to schedule the installation
  name: schedule
  type: string
- description: Schema synchronization mode
  name: schemaSyncMode
  type: string
- description: ''
  name: status
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-extension-upload-schema.json
slug: automation-extension-upload
source_filename: automation-extension-upload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExtensionUpload\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"systemId\": {\n      \"type\": \"string\"\n    },\n    \"schedule\": {\n      \"type\": \"string\",\n      \"description\": \"When to schedule the installation\"\n    },\n    \"schemaSyncMode\": {\n      \"type\": \"string\",\n      \"description\": \"Schema synchronization mode\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-extension-upload-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: ExtensionUpload
---
