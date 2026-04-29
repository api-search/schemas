---
description: A Power Automate connector.
layout: schema
name: Connector
properties_list:
- description: The connector name.
  name: name
  type: string
- description: ''
  name: properties
  type: object
provider_name: Microsoft Power Automate
provider_slug: microsoft-power-automate
schema_file: json-schema/power-automate-management-api-connector-schema.json
slug: power-automate-management-api-connector
source_filename: power-automate-management-api-connector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/json-schema/power-automate-management-api-connector-schema.json\",\n  \"title\": \"Connector\",\n  \"description\": \"A Power Automate connector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": { \"type\": \"string\", \"description\": \"The connector name.\" },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"displayName\": { \"type\": \"string\" },\n        \"iconUri\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"isCustomApi\": { \"type\": \"boolean\" },\n        \"tier\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-automate/refs/heads/main/json-schema/power-automate-management-api-connector-schema.json
tags:
- Automation
- Business Process
- Integration
- Low-Code
- Microsoft
- Power Platform
- RPA
- Workflow
title: Connector
---
