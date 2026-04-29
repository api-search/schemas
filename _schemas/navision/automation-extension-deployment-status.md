---
description: ''
layout: schema
name: ExtensionDeploymentStatus
properties_list:
- description: ''
  name: id
  type: string
- description: Extension name
  name: name
  type: string
- description: Extension publisher
  name: publisher
  type: string
- description: Type of deployment operation
  name: operationType
  type: string
- description: Deployment status
  name: status
  type: string
- description: Extension version
  name: appVersion
  type: string
- description: ''
  name: startedOn
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/automation-extension-deployment-status-schema.json
slug: automation-extension-deployment-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExtensionDeploymentStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Extension name\"\n    },\n    \"publisher\": {\n      \"type\": \"string\",\n      \"description\": \"Extension publisher\"\n    },\n    \"operationType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of deployment operation\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment status\"\n    },\n    \"appVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Extension version\"\n    },\n    \"startedOn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/automation-extension-deployment-status-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: ExtensionDeploymentStatus
---
