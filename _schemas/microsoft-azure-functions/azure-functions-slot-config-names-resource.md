---
description: Slot Config names azure resource.
layout: schema
name: SlotConfigNamesResource
properties_list:
- description: Core resource properties
  name: properties
  type: object
- description: Kind of resource.
  name: kind
  type: string
provider_name: Microsoft Azure Functions
provider_slug: microsoft-azure-functions
schema_file: json-schema/azure-functions-slot-config-names-resource-schema.json
slug: azure-functions-slot-config-names-resource
source_filename: azure-functions-slot-config-names-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-slot-config-names-resource-schema.json\",\n  \"title\": \"SlotConfigNamesResource\",\n  \"description\": \"Slot Config names azure resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/SlotConfigNames\",\n      \"description\": \"Core resource properties\",\n      \"x-ms-client-flatten\": true\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-functions/refs/heads/main/json-schema/azure-functions-slot-config-names-resource-schema.json
tags:
- Azure
- Cloud
- Compute
- Event-Driven
- Microsoft
- Serverless
title: SlotConfigNamesResource
---
