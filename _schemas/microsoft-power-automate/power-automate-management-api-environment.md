---
description: A Power Automate environment.
layout: schema
name: Environment
properties_list:
- description: The unique name of the environment.
  name: name
  type: string
- description: The geographic location.
  name: location
  type: string
- description: ''
  name: properties
  type: object
provider_name: Microsoft Power Automate
provider_slug: microsoft-power-automate
schema_file: json-schema/power-automate-management-api-environment-schema.json
slug: power-automate-management-api-environment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/json-schema/power-automate-management-api-environment-schema.json\",\n  \"title\": \"Environment\",\n  \"description\": \"A Power Automate environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": { \"type\": \"string\", \"description\": \"The unique name of the environment.\" },\n    \"location\": { \"type\": \"string\", \"description\": \"The geographic location.\" },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayName\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" },\n        \"createdTime\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"lastModifiedTime\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"provisioningState\": { \"type\": \"string\" },\n        \"environmentSku\"\
  : { \"type\": \"string\" },\n        \"environmentType\": { \"type\": \"string\" },\n        \"isDefault\": { \"type\": \"boolean\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/json-schema/power-automate-management-api-environment-schema.json
tags:
- Automation
- Business Process
- Integration
- Low-Code
- Microsoft
- Power Platform
- RPA
- Workflow
title: Environment
---
